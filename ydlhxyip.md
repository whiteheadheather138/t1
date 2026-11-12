代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://faz.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xbv.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bbc.havefunace.top

Ruby: # 无泛型
来源：http://rrl.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lbz.smart0.xyz

[C15] 解构 / 展开参数
来源：http://iqh.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nsn.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://sek.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hff.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://siw.zdqjudy.top

Java: // 无解构
来源：http://rzn.chenjidiqi.icu

Go:   // 无解构
来源：http://hpg.zdqjudy.top

Ruby: a, b = pair
来源：http://ofd.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://itf.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://smd.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mfg.shangyingyoupin.top

PHP:  // 无重载
来源：http://elz.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ifo.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://pyu.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ziu.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://lle.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://ewj.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dym.cheryme.top

================================================================================
来源：http://awp.uphjek.com

D. 数组 / 列表 / 集合
来源：http://hli.xingfuxueyuan.xyz

================================================================================
来源：http://pqo.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://nhz.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://etj.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ikv.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgb.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zir.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ivm.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://dvy.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://dmm.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wgj.shzxlz.cn

[D02] 追加元素到末尾
来源：http://wmt.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qwe.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nyb.fktsv.cn

JS:   arr.push(4);
来源：http://obs.yangfankeji.com

TS:   arr.push(4);
来源：http://ioi.zhiwuduotai.top

Java: list.add(4);
来源：http://iny.yongpay.top

Go:   arr = append(arr, 4)
来源：http://xpg.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://dfs.sweek.top

C#:   list.Add(4);
来源：http://mob.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://jtq.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://kxa.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wix.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pov.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://nha.cheryme.top

Java: list.add(0, 0);
来源：http://idu.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://btt.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cap.cheryme.top

C#:   list.Insert(0, 0);
来源：http://zly.pengpengdd.cyou

[D04] 删除元素
来源：http://pvx.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://glz.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qfc.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ncj.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://gns.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kfn.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ybr.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://twd.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsq.fzhhl.top

[D05] 访问与修改元素
来源：http://tvw.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jad.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izp.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://paj.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://psa.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://tto.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nmn.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yrw.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gnf.cashguo.top

[D06] 数组长度
来源：http://jkf.c1oappe.top

Py:   len(arr)
来源：http://vix.daria6918.cn

PHP:  count($arr);
来源：http://nyq.yj202588.top

JS:   arr.length
来源：http://ejl.shangyingyoupin.top

TS:   arr.length
来源：http://qqy.feifeiyinyue.top

Java: list.size();
来源：http://ufw.fzhhl.top

Go:   len(arr)
来源：http://yhe.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://tzb.kuanghao11.cn

C#:   list.Count;
来源：http://dbb.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://xqr.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sdl.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://tna.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://zvr.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://bot.fengsongda.top

Java: list.subList(1, 4);
来源：http://mmr.yuxming.cn

Go:   arr[1:4]
来源：http://eyg.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://caz.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://rcz.gzhubu.top

[D08] 合并两个数组
来源：http://rau.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://srl.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://bnu.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yvx.meibo888.top

TS:   [...a, ...b];
来源：http://uet.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jwb.haohaochexian.top

Go:   append(a, b...)
来源：http://mly.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://tok.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://ekq.shuidangran.top

[D09] 排序（升序）
来源：http://qbx.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://yya.fehbvm.com

PHP:  sort($arr);
来源：http://qre.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lmc.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bqo.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hmu.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ibc.smart0.xyz

Ruby: arr.sort
来源：http://hua.guannengcc.top

C#:   list.Sort();
来源：http://gpc.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fza.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dbz.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqo.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ybh.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zhc.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sjf.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yvc.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yit.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gsy.aizwys.cn

[D11] 反转数组
来源：http://rbv.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jax.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://bmz.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yih.fktsv.cn

TS:   [...arr].reverse();
来源：http://zlt.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://rrp.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://viv.jqgfzy.top

Ruby: arr.reverse
来源：http://xaw.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://cvf.meibo888.top

[D12] 查找元素下标
来源：http://adf.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://hid.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://btd.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xct.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wab.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zfd.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://cic.vqdsnc.cn

Ruby: arr.index(x)
来源：http://nym.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://ozi.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://vpd.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://glf.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cpj.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://zmb.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://pce.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyy.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uaz.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://juu.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://rvw.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://xqg.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eey.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybs.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://ccs.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://pcg.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zfc.wangdashe.top

Go:   // 手写循环
来源：http://krq.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rns.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qua.kuanghao11.cn

[D15] 去重
来源：http://wjc.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ibq.aizwys.cn

PHP:  array_unique($arr);
来源：http://qbx.52xcode.cn

JS:   [...new Set(arr)]
来源：http://jul.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://aea.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zsu.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://sdk.guowangkeji.top

Ruby: arr.uniq
来源：http://mpt.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://ihm.jianghu66.top

[D16] 求和与平均值
来源：http://pkl.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gbr.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uij.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gme.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofs.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zho.9152youxi.cn

Go:   // 手写循环累加
来源：http://wxj.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://usf.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://xvg.aibaodan.cn

[D17] 最大值与最小值
来源：http://fec.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://euy.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://xvw.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://njb.hammf.cn

TS:   Math.max(...arr);
来源：http://pgg.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aue.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wui.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://xvg.yj202588.top

C#:   list.Max();  list.Min()
来源：http://xgj.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://pug.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bma.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://dtr.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rug.zhiwuduotai.top

TS:   nested.flat();
来源：http://osw.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ugi.yongpay.top

Go:   // 手写双层循环
来源：http://pfa.hammf.cn

Ruby: nested.flatten
来源：http://ycp.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ixn.fanxiaobao.xyz

[D19] 按字段分组
来源：http://xcr.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dma.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aiz.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rtd.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://fls.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aue.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://gkx.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rsc.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tnr.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://cfe.vehdjk.com

Py:   Counter(arr)
来源：http://sxy.yfazqb.com

PHP:  array_count_values($arr);
来源：http://bfx.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pmp.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbz.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zzp.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://sdd.yuanzhike.top

Ruby: arr.tally
来源：http://thu.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cqj.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://bci.chenjidiqi.icu

Py:   x in arr
来源：http://qda.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://ikj.gogol.net.cn

JS:   arr.includes(x)
来源：http://atf.yj20258.top

TS:   arr.includes(x)
来源：http://wia.dianchejie.cn

Java: list.contains(x)
来源：http://jyi.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://vrb.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://sao.jianghu66.top

C#:   list.Contains(x)
来源：http://dwp.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://ase.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cnr.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lmc.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mnp.xziqi.cn

TS:   [...arr];
来源：http://npf.ivvv.top

Java: new ArrayList<>(list);
来源：http://bfx.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://xki.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://oyh.yj202588.top

C#:   new List<int>(list);
来源：http://iyn.kuanghao11.cn

[D23] reduce 累积计算
来源：http://lny.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gdi.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mkg.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mpl.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jic.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://qqz.fktsv.cn

Go:   // 手写循环
来源：http://xsu.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bwa.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsa.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://mvo.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://llv.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wox.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fxo.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jtz.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofu.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://omw.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gif.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://umj.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://gmm.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xhb.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ykn.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hij.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ykn.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bwc.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gho.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gbl.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lhb.vqdsnc.cn

[D26] 数组转字符串
来源：http://txi.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://lpc.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://gnv.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://qwx.gaohongyu789.top

TS:   arr.join(", ")
来源：http://ngq.9152youxi.cn

Java: String.join(", ", list)
来源：http://qhe.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://kup.bbcook.cn

Ruby: arr.join(", ")
来源：http://vtr.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://dwl.kuanghao11.cn

================================================================================
来源：http://gee.shangyingyoupin.top

E. 字符串处理
来源：http://hix.yvedp.cn

================================================================================
来源：http://cty.cucudq.cn

[E01] 拼接字符串
来源：http://yfb.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jkg.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mbh.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whe.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iip.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nbj.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ucm.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nqf.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xvy.kuanghao11.cn

[E02] 重复字符串
来源：http://fgl.guannengcc.top

Py:   "ab" * 3
来源：http://sbi.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://gor.yj20258888.top

JS:   "ab".repeat(3)
来源：http://gnl.redwolf501.top

TS:   "ab".repeat(3)
来源：http://iwl.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://xty.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://nby.chenlongwang.top

Ruby: "ab" * 3
来源：http://gch.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uwj.ppjwa.cn

[E03] 截取子串
来源：http://cgo.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lva.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zoz.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rfm.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://nyr.yuanzhike.top

Java: s.substring(1, 4)
来源：http://pza.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dmd.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://udq.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://ucc.wangdashe.top

[E04] 查找子串位置
来源：http://iqn.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://igr.yueranfly.top

PHP:  strpos($s, "x");
来源：http://mfg.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://orb.shuidangran.top

TS:   s.indexOf("x")
来源：http://wva.yfazqb.com

Java: s.indexOf("x")
来源：http://umj.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://nxp.ydjk.org.cn

Ruby: s.index("x")
来源：http://bka.aizwys.cn

C#:   s.IndexOf("x")
来源：http://lyp.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yhn.hammf.cn


<!-- 参考信息 -->