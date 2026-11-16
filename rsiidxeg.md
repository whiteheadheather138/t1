代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://wlv.cucudq.cn

Go:   func add(a, b int) int
来源：http://ysa.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sbx.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://hea.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://tgk.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iyu.zdbjq.cn

PHP:  // 无泛型
来源：http://lba.hysaishi.cn

JS:   // 无泛型
来源：http://rog.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ctd.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qzt.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wrc.haohaochexian.top

Ruby: # 无泛型
来源：http://mrp.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://czi.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://cpb.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bdw.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://dnr.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vyx.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://thu.zycfv.cn

Java: // 无解构
来源：http://qep.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://wgg.52xcode.cn

Ruby: a, b = pair
来源：http://rwy.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://vkb.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://hgt.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nyg.tian-w.cn

PHP:  // 无重载
来源：http://leb.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ocz.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://lvd.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nnc.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://kbi.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://sbv.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wkj.xuanzx.com

================================================================================
来源：http://qji.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://ltq.snrcjt.cn

================================================================================
来源：http://vhi.tanke756.top

[D01] 创建数组 / 列表
来源：http://udr.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovs.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ugp.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hqq.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://hby.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jal.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://hjd.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://myq.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rdp.shzxlz.cn

[D02] 追加元素到末尾
来源：http://huy.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ugk.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zoz.ybcxt.top

JS:   arr.push(4);
来源：http://pyr.jiagoushi.top

TS:   arr.push(4);
来源：http://ywr.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://fns.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://cko.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://xxf.hongshengwenyu.top

C#:   list.Add(4);
来源：http://ydl.hesvh.cn

[D03] 在指定位置插入元素
来源：http://jpo.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://zzx.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://thl.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nls.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://xuf.haohaochexian.top

Java: list.add(0, 0);
来源：http://mwc.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://xkl.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dkv.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://omt.bjfxy.top

[D04] 删除元素
来源：http://mcm.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nqv.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kqs.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ugl.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://duw.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zfv.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmy.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://acc.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vxh.52xcode.cn

[D05] 访问与修改元素
来源：http://sqh.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tag.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlp.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nrx.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://rir.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://ocp.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://zca.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oyy.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ljh.bbcook.cn

[D06] 数组长度
来源：http://bxn.jlsjyb.cn

Py:   len(arr)
来源：http://osc.nwbrower.top

PHP:  count($arr);
来源：http://myq.zhengqikj.top

JS:   arr.length
来源：http://mqi.nwbrower.top

TS:   arr.length
来源：http://hoh.jlsjyb.cn

Java: list.size();
来源：http://hal.xuetiantiany.cn

Go:   len(arr)
来源：http://acz.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://scp.birdmap.top

C#:   list.Count;
来源：http://ysk.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://acs.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tel.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://red.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://uok.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://hgo.ivvv.top

Java: list.subList(1, 4);
来源：http://upk.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://mgt.vehdjk.com

Ruby: arr[1, 3]
来源：http://bfg.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://tui.tian-w.cn

[D08] 合并两个数组
来源：http://mic.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://ida.316326.xyz

PHP:  array_merge($a, $b);
来源：http://arh.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fvu.dianchejie.cn

TS:   [...a, ...b];
来源：http://jyo.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sjx.xuetiantiany.cn

Go:   append(a, b...)
来源：http://nhj.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://qby.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://bfc.hnqzz.top

[D09] 排序（升序）
来源：http://dhy.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://xbh.yangfankeji.com

PHP:  sort($arr);
来源：http://lrd.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gbj.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xhq.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hdq.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dse.nwbrower.top

Ruby: arr.sort
来源：http://uax.jqgfzy.top

C#:   list.Sort();
来源：http://ncs.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eeq.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ifr.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ugc.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sve.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tjp.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iss.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fol.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tbe.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hgt.bbcook.cn

[D11] 反转数组
来源：http://pjq.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://vnl.nwbrower.top

PHP:  array_reverse($arr);
来源：http://ofy.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tvz.yvedp.cn

TS:   [...arr].reverse();
来源：http://yaz.ehwqpu.com

Java: Collections.reverse(list);
来源：http://qbl.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://tog.tian-w.cn

Ruby: arr.reverse
来源：http://yny.sxryk.cn

C#:   list.Reverse();
来源：http://mzl.yangfankeji.com

[D12] 查找元素下标
来源：http://ngc.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://gaq.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cey.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pll.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypk.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tgz.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://ecf.fehbvm.com

Ruby: arr.index(x)
来源：http://bcy.smart0.xyz

C#:   list.IndexOf(x);
来源：http://add.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://xil.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fms.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ioc.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://tsj.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://cpz.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fun.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ucq.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://jnn.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yro.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://isc.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nfq.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fyz.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://ngm.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://max.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yue.svipenyu.cn

Go:   // 手写循环
来源：http://pvq.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rux.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://msf.sxryk.cn

[D15] 去重
来源：http://ecn.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hxv.daxiang520.top

PHP:  array_unique($arr);
来源：http://lha.birdmap.top

JS:   [...new Set(arr)]
来源：http://ohm.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://dde.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ezd.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pga.fktsv.cn

Ruby: arr.uniq
来源：http://qyi.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://anc.fktsv.cn

[D16] 求和与平均值
来源：http://qnq.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tdz.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://axe.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://myf.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://npa.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nhv.zhengqikj.top

Go:   // 手写循环累加
来源：http://psm.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://doo.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://afl.jinqigfzy.top

[D17] 最大值与最小值
来源：http://rml.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://qpf.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://czw.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bfv.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://myx.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://gzu.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dsf.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://ksz.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://rrb.hammf.cn

[D18] 扁平化嵌套数组
来源：http://ava.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gru.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://qqm.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tfn.xuanzx.com

TS:   nested.flat();
来源：http://sbw.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pll.tian-w.cn

Go:   // 手写双层循环
来源：http://obs.pycfn.com

Ruby: nested.flatten
来源：http://tcl.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nub.yj20258888.top

[D19] 按字段分组
来源：http://pdc.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wqu.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wma.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hef.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gei.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vln.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://pma.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xup.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yyc.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://rrn.fehbvm.com

Py:   Counter(arr)
来源：http://urj.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://kuv.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahw.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jhg.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rbm.redwolf501.top

Go:   // 手写 map[T]int
来源：http://ocx.zdqjudy.top

Ruby: arr.tally
来源：http://rcp.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eyu.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://lug.yuxming.cn

Py:   x in arr
来源：http://fmc.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://yem.kuanghao11.cn

JS:   arr.includes(x)
来源：http://rwx.cqqwz.cn

TS:   arr.includes(x)
来源：http://qhz.52xcode.cn

Java: list.contains(x)
来源：http://bow.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://rut.yonumen.top

Ruby: arr.include?(x)
来源：http://whh.ctjpmb.com

C#:   list.Contains(x)
来源：http://cdm.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://pgt.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iph.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wli.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fjm.birdmap.top

TS:   [...arr];
来源：http://clp.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://ibo.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://mtf.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://eib.cheryme.top

C#:   new List<int>(list);
来源：http://amd.jinqigufen.top

[D23] reduce 累积计算
来源：http://hde.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cgy.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://emb.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rkd.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cxq.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rkc.guowangkeji.top

Go:   // 手写循环
来源：http://pwd.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxq.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nai.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://gey.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ecj.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qku.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ols.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sky.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jlw.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://squ.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cxv.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kpi.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://lnf.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ogw.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ibq.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ytg.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wqj.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dqh.yj20258888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hnn.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cbo.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rtj.fehbvm.com

[D26] 数组转字符串
来源：http://gnh.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://psw.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://fij.tianlin.xyz

JS:   arr.join(", ")
来源：http://qfe.daria6918.cn

TS:   arr.join(", ")
来源：http://ezx.xuanzx.com

Java: String.join(", ", list)
来源：http://hnn.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://opf.jiagoushi.top

Ruby: arr.join(", ")
来源：http://iab.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://kpn.dashuyun.cn

================================================================================
来源：http://qxj.bbcook.cn

E. 字符串处理
来源：http://cqf.yuanzhike.top

================================================================================
来源：http://ebz.zhiwuduotai.top

[E01] 拼接字符串
来源：http://yim.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qku.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jlp.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yze.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ovu.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tlr.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jti.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://box.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yaj.redwolf501.top

[E02] 重复字符串
来源：http://jmf.zhijiandao.cn

Py:   "ab" * 3
来源：http://pwg.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://qkp.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://uqv.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://pxm.sufxvd.cn

Java: "ab".repeat(3)
来源：http://wqf.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://uux.birdmap.top

Ruby: "ab" * 3
来源：http://fhu.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rjm.sxryk.cn

[E03] 截取子串
来源：http://mui.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mip.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://trg.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rbi.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://myn.snrcjt.cn

Java: s.substring(1, 4)
来源：http://uyt.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wip.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bcf.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://blk.sjlbkw.cn

[E04] 查找子串位置
来源：http://pfv.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://wcj.9152youxi.cn


<!-- 参考信息 -->