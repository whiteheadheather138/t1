代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://evs.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://tfj.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zsu.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://mzl.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vnh.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qkj.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cax.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zrx.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://ucm.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://ech.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oxp.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://wln.redwolf501.top

[C14] 泛型函数
来源：http://hoo.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kmp.yuxming.cn

PHP:  // 无泛型
来源：http://zda.zhengqikj.top

JS:   // 无泛型
来源：http://ftn.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pud.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mpm.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ewp.vehdjk.com

Ruby: # 无泛型
来源：http://btu.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vax.xuanzx.com

[C15] 解构 / 展开参数
来源：http://iit.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhz.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://qcx.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nqb.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fgc.shanyushiyangkeji.top

Java: // 无解构
来源：http://pnp.hongshengwenyu.top

Go:   // 无解构
来源：http://kqi.zycfv.cn

Ruby: a, b = pair
来源：http://rnv.daxiang520.top

C#:   var (a, b) = pair;
来源：http://ztr.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://czy.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qeh.mhx1999.top

PHP:  // 无重载
来源：http://zck.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ipr.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://vci.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qdv.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://spg.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://ygf.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zhz.sxryk.cn

================================================================================
来源：http://kiz.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://alp.c1oappe.top

================================================================================
来源：http://hur.andypj.xyz

[D01] 创建数组 / 列表
来源：http://zev.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xhn.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blf.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jkm.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eqs.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nhe.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://czp.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://kxq.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pyt.cucudq.cn

[D02] 追加元素到末尾
来源：http://xug.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwk.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zcg.wangdashe.top

JS:   arr.push(4);
来源：http://teu.birdmap.top

TS:   arr.push(4);
来源：http://sjp.0kj1m.cn

Java: list.add(4);
来源：http://unm.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://myt.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://red.wangshuangyany.cn

C#:   list.Add(4);
来源：http://qdx.iojbl.cn

[D03] 在指定位置插入元素
来源：http://pmi.ivvv.top

Py:   arr.insert(0, 0)
来源：http://zfw.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://npv.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wfl.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://elu.yangfankeji.com

Java: list.add(0, 0);
来源：http://fel.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://dxf.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qwf.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://ucc.fanxiaobao.xyz

[D04] 删除元素
来源：http://klj.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xjr.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dik.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iqr.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://own.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsd.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wws.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://obx.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jmz.vqdsnc.cn

[D05] 访问与修改元素
来源：http://jak.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pax.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pbe.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sxu.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://rze.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://vab.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://hns.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nzz.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tgq.daxiang520.top

[D06] 数组长度
来源：http://bmd.fengsongda.top

Py:   len(arr)
来源：http://ahg.nwbrower.top

PHP:  count($arr);
来源：http://klj.ydzc1.top

JS:   arr.length
来源：http://nrb.316326.xyz

TS:   arr.length
来源：http://ois.yfazqb.com

Java: list.size();
来源：http://ujg.tian-w.cn

Go:   len(arr)
来源：http://col.gzhubu.top

Ruby: arr.length; arr.size
来源：http://mkk.jyoumei.cn

C#:   list.Count;
来源：http://xua.birdmap.top

[D07] 切片 / 取子数组
来源：http://ozu.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://krc.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://peo.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://tmf.ivvv.top

TS:   arr.slice(1, 4);
来源：http://fvo.jinqigufen.top

Java: list.subList(1, 4);
来源：http://pga.zhoulong.xyz

Go:   arr[1:4]
来源：http://wca.gotoacloud.top

Ruby: arr[1, 3]
来源：http://brb.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://csx.fengsongda.top

[D08] 合并两个数组
来源：http://mpf.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://vnz.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://sxz.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wim.jyoumei.cn

TS:   [...a, ...b];
来源：http://dda.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qpu.9152youxi.cn

Go:   append(a, b...)
来源：http://nrq.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://oad.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://dqs.wangdashe.top

[D09] 排序（升序）
来源：http://nxm.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://huq.shuidangran.top

PHP:  sort($arr);
来源：http://xls.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://duy.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ojv.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yeb.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://los.hywenlv.cn

Ruby: arr.sort
来源：http://yyp.zhengqikj.top

C#:   list.Sort();
来源：http://pkb.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aeg.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xgq.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lig.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://djb.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gkk.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cuv.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sxi.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xmo.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nsv.ctjpmb.com

[D11] 反转数组
来源：http://ggs.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sey.shuidangran.top

PHP:  array_reverse($arr);
来源：http://nza.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qlf.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://dfg.bjfxy.top

Java: Collections.reverse(list);
来源：http://kbz.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://qbr.fengsongda.top

Ruby: arr.reverse
来源：http://lfr.yanxiufei.cn

C#:   list.Reverse();
来源：http://dpl.kuanghao11.cn

[D12] 查找元素下标
来源：http://bus.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://qfp.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dqq.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzj.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdb.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mhk.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://wua.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://zdu.smart0.xyz

C#:   list.IndexOf(x);
来源：http://bqm.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://bat.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xut.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fpf.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://qzq.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://iil.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eut.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zcm.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://hob.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bef.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://kwx.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xvc.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uxv.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://oxt.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://coo.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qil.fanxiaobao.xyz

Go:   // 手写循环
来源：http://yuy.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://eav.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://unn.tian-w.cn

[D15] 去重
来源：http://vrd.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://edc.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://zkj.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://dlr.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://phg.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sfn.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tnl.vehdjk.com

Ruby: arr.uniq
来源：http://wpp.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://rak.xuanzx.com

[D16] 求和与平均值
来源：http://kpc.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vzj.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ftc.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibu.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mjx.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rae.chenzaomai.com

Go:   // 手写循环累加
来源：http://fnv.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ozl.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://mqk.sweek.top

[D17] 最大值与最小值
来源：http://hkw.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://yvs.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://eqd.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lna.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://asn.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ega.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymk.ivvv.top

Ruby: arr.max;  arr.min
来源：http://oyp.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://uxl.yonumen.top

[D18] 扁平化嵌套数组
来源：http://mnf.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lrw.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://rrj.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tbb.ppjwa.cn

TS:   nested.flat();
来源：http://kfo.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xcj.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://btu.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://vyn.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cxq.chenzaomai.com

[D19] 按字段分组
来源：http://kkx.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wfc.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xly.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://msx.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nyz.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dhf.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://bal.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://zzo.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lft.tanke756.top

[D20] 统计每个元素出现次数
来源：http://shi.cqqwz.cn

Py:   Counter(arr)
来源：http://ewn.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://zwd.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkr.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msa.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rei.fktsv.cn

Go:   // 手写 map[T]int
来源：http://dwr.pycfn.com

Ruby: arr.tally
来源：http://ilz.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yli.daxiang520.top

[D21] 判断是否包含某元素
来源：http://dro.havefunace.top

Py:   x in arr
来源：http://jmh.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://mib.zhengqikj.top

JS:   arr.includes(x)
来源：http://pqk.shzxlz.cn

TS:   arr.includes(x)
来源：http://bjo.hammf.cn

Java: list.contains(x)
来源：http://vix.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://kod.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://tqk.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://rrc.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://swg.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kbd.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mmc.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tls.fzhhl.top

TS:   [...arr];
来源：http://uha.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://jdp.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://dsa.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://svo.yuxming.cn

C#:   new List<int>(list);
来源：http://lcz.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://nat.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aki.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tqe.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gtl.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wgv.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://zui.vehdjk.com

Go:   // 手写循环
来源：http://dvm.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ioy.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uqa.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://wvy.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qsy.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://trr.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aik.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ewn.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kbh.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bby.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bhk.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://onf.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://kbm.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://neu.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ywo.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://moj.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gpy.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bql.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mdp.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://onn.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vyd.9152youxi.cn

[D26] 数组转字符串
来源：http://yxg.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://tqv.pycfn.com

PHP:  implode(", ", $arr);
来源：http://wjk.yanxiufei.cn

JS:   arr.join(", ")
来源：http://mde.nanxinkj.top

TS:   arr.join(", ")
来源：http://oui.meibo888.top

Java: String.join(", ", list)
来源：http://yav.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://qih.uphjek.com

Ruby: arr.join(", ")
来源：http://vzq.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://pvv.pycfn.com

================================================================================
来源：http://pix.xuanzx.com

E. 字符串处理
来源：http://rxn.zycfv.cn

================================================================================
来源：http://mvb.yuxming.cn

[E01] 拼接字符串
来源：http://kvl.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zaj.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://owa.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nkr.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoj.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wzi.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dvi.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rzo.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jbm.jinghuilouyu.cn

[E02] 重复字符串
来源：http://ojm.shuidangran.top

Py:   "ab" * 3
来源：http://bsj.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://ehy.sysykeji.top

JS:   "ab".repeat(3)
来源：http://iqh.ydzc1.top

TS:   "ab".repeat(3)
来源：http://afw.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://ntv.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://hzf.zdbjq.cn

Ruby: "ab" * 3
来源：http://pxs.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wnh.hammf.cn

[E03] 截取子串
来源：http://evo.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hus.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tsx.tianlin.xyz


<!-- 参考信息 -->