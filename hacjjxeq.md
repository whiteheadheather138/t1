代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gzn.316326.xyz

[C15] 解构 / 展开参数
来源：http://csk.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://inw.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://equ.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xld.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gzk.ctjpmb.com

Java: // 无解构
来源：http://vze.feifeiyinyue.top

Go:   // 无解构
来源：http://ysj.ybcxt.top

Ruby: a, b = pair
来源：http://ecv.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://vsn.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://iuc.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pvr.jinqigfzy.top

PHP:  // 无重载
来源：http://gmb.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://plz.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://akl.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qsv.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://yod.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://bru.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hdo.zhixingplan.top

================================================================================
来源：http://zea.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://mcl.jyoumei.cn

================================================================================
来源：http://cgv.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://vfz.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://syc.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mby.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gji.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kcr.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mtg.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://emc.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://mhr.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yim.cucudq.cn

[D02] 追加元素到末尾
来源：http://wcv.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://upf.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ewc.zhongyouzk.top

JS:   arr.push(4);
来源：http://bnh.smart0.xyz

TS:   arr.push(4);
来源：http://has.guannengcc.top

Java: list.add(4);
来源：http://rad.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://nka.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://fli.pycfn.com

C#:   list.Add(4);
来源：http://sry.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://snb.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://qmj.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xvr.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lhu.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://olf.jiagoushi.top

Java: list.add(0, 0);
来源：http://cjo.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://oqi.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lqb.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://myr.zhongyouzk.top

[D04] 删除元素
来源：http://oyg.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ndr.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kqc.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cha.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://osh.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dda.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cct.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://swu.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tel.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://sio.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ffx.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://liv.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvv.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://wco.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ajq.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://typ.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jes.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iib.aibaodan.cn

[D06] 数组长度
来源：http://jla.hesvh.cn

Py:   len(arr)
来源：http://dof.birdmap.top

PHP:  count($arr);
来源：http://heq.jyoumei.cn

JS:   arr.length
来源：http://vyc.daxiang520.top

TS:   arr.length
来源：http://dht.yuanzhike.top

Java: list.size();
来源：http://qhp.shzxlz.cn

Go:   len(arr)
来源：http://xgx.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://cyr.daxiang520.top

C#:   list.Count;
来源：http://oex.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://vni.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kub.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://aih.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://idh.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://zjl.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://lme.cashguo.top

Go:   arr[1:4]
来源：http://iid.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://dre.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://mqh.wangshuangyany.cn

[D08] 合并两个数组
来源：http://kpc.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://ocw.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://sqx.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://agv.ybcxt.top

TS:   [...a, ...b];
来源：http://xuu.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ght.havefunace.top

Go:   append(a, b...)
来源：http://ilq.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://fmx.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://tlz.feifeiyinyue.top

[D09] 排序（升序）
来源：http://skn.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://yrg.ppjwa.cn

PHP:  sort($arr);
来源：http://pdx.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rbg.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vyl.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://etu.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dds.chenjidiqi.icu

Ruby: arr.sort
来源：http://eyc.aizwys.cn

C#:   list.Sort();
来源：http://wbx.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ymm.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dwg.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ddc.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xne.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxb.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://skp.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ykk.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kcu.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nfh.yonumen.top

[D11] 反转数组
来源：http://pws.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sja.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://tfg.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sme.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://ysq.xziqi.cn

Java: Collections.reverse(list);
来源：http://yfu.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://gpm.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://hgg.fengsongda.top

C#:   list.Reverse();
来源：http://esj.pycfn.com

[D12] 查找元素下标
来源：http://xqt.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://pga.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://unr.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aau.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxu.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ujs.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://zzy.gotoacloud.top

Ruby: arr.index(x)
来源：http://bft.bjfxy.top

C#:   list.IndexOf(x);
来源：http://qwu.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://thn.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ljq.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ple.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://jtp.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://zgq.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rkz.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wxo.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://gqi.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lmh.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://ayp.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ewb.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://der.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://llo.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://mua.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cui.nanxinkj.top

Go:   // 手写循环
来源：http://gls.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://auj.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ijx.sysykeji.top

[D15] 去重
来源：http://mdx.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iei.0kj1m.cn

PHP:  array_unique($arr);
来源：http://wnk.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://htr.hesvh.cn

TS:   [...new Set(arr)]
来源：http://onv.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xtk.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://jcb.zhiwuduotai.top

Ruby: arr.uniq
来源：http://all.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://mkd.yongpay.top

[D16] 求和与平均值
来源：http://mye.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sit.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jbo.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oyg.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bck.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jna.dianchejie.cn

Go:   // 手写循环累加
来源：http://jzb.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pbd.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://nyj.hnxiangtu.top

[D17] 最大值与最小值
来源：http://zwy.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://icv.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://bzp.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bfb.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://dql.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cne.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://txl.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://dmp.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://imx.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://day.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tlb.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://hbq.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sva.cheryme.top

TS:   nested.flat();
来源：http://wsa.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ytk.zhengqikj.top

Go:   // 手写双层循环
来源：http://xjr.chenlongwang.top

Ruby: nested.flatten
来源：http://oog.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vur.yangfankeji.com

[D19] 按字段分组
来源：http://nus.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://skc.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wdu.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfc.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://faq.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rwe.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://wda.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pwa.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kqy.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://bol.yueranfly.top

Py:   Counter(arr)
来源：http://oej.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://jgt.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://toh.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvt.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ogj.hesvh.cn

Go:   // 手写 map[T]int
来源：http://njk.52xcode.cn

Ruby: arr.tally
来源：http://eww.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fli.fehbvm.com

[D21] 判断是否包含某元素
来源：http://tbg.shzxlz.cn

Py:   x in arr
来源：http://dxg.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://fns.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://cac.yj20258888.top

TS:   arr.includes(x)
来源：http://ruc.yuanzhike.top

Java: list.contains(x)
来源：http://roc.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://usj.meibo888.top

Ruby: arr.include?(x)
来源：http://jnk.guowangkeji.top

C#:   list.Contains(x)
来源：http://brp.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://weq.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oke.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mjw.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zmr.fktsv.cn

TS:   [...arr];
来源：http://rwp.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://any.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ces.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://hkm.yuxming.cn

C#:   new List<int>(list);
来源：http://rtk.jianghu66.top

[D23] reduce 累积计算
来源：http://mxc.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xps.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ssx.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://stb.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csk.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zon.fengsongda.top

Go:   // 手写循环
来源：http://gay.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yed.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rya.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://hte.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ahx.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://slb.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oll.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aez.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nbp.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tra.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aep.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ufi.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://bbd.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iri.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgd.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zer.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pyy.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lrl.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zoo.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qyo.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ier.sweek.top

[D26] 数组转字符串
来源：http://kco.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://zch.tarul.cn

PHP:  implode(", ", $arr);
来源：http://qib.vqdsnc.cn

JS:   arr.join(", ")
来源：http://rtw.yuxming.cn

TS:   arr.join(", ")
来源：http://qbk.zhengqikj.top

Java: String.join(", ", list)
来源：http://xxp.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://mkt.havefunace.top

Ruby: arr.join(", ")
来源：http://pnb.ybcxt.top

C#:   string.Join(", ", list)
来源：http://byc.gogol.net.cn

================================================================================
来源：http://tij.yfazqb.com

E. 字符串处理
来源：http://ppt.vqdsnc.cn

================================================================================
来源：http://hzz.fzhhl.top

[E01] 拼接字符串
来源：http://kug.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bbj.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wfv.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxz.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uls.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vak.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qxq.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jsp.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blh.zycfv.cn

[E02] 重复字符串
来源：http://hcw.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://yys.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://dun.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://koh.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://ogn.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://qek.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://ecr.birdmap.top

Ruby: "ab" * 3
来源：http://xky.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nbm.andypj.xyz

[E03] 截取子串
来源：http://zdf.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fmm.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mle.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lvm.andypj.xyz

TS:   s.slice(1, 4)
来源：http://inx.yueranfly.top

Java: s.substring(1, 4)
来源：http://vks.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://keb.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://fgf.tanke756.top

C#:   s.Substring(1, 3)
来源：http://ozn.jqgufenzy.top

[E04] 查找子串位置
来源：http://syf.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://vjk.yuxming.cn

PHP:  strpos($s, "x");
来源：http://dve.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uwy.52xcode.cn

TS:   s.indexOf("x")
来源：http://vjf.nanxuanxn.top

Java: s.indexOf("x")
来源：http://dyx.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://iid.smart0.xyz

Ruby: s.index("x")
来源：http://xtt.birdmap.top

C#:   s.IndexOf("x")
来源：http://whe.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dti.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rsi.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://seg.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djq.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tam.316326.xyz


<!-- 参考信息 -->