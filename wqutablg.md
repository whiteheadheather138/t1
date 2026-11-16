代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://hkl.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://tvk.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rxq.chenlongwang.top

================================================================================
来源：http://dqx.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://ugq.hnqzz.top

================================================================================
来源：http://ehb.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://exp.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ivk.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vca.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yal.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fqx.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vdk.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://gui.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://hkg.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fsy.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://ivi.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vpw.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xas.snrcjt.cn

JS:   arr.push(4);
来源：http://vja.ehwqpu.com

TS:   arr.push(4);
来源：http://gse.pengpengdd.cyou

Java: list.add(4);
来源：http://zpr.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://ian.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://aun.xziqi.cn

C#:   list.Add(4);
来源：http://ltc.jianghu66.top

[D03] 在指定位置插入元素
来源：http://izh.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://ukf.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rts.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yhg.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://yfi.yueranfly.top

Java: list.add(0, 0);
来源：http://exm.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://gca.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpi.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://dgo.zycfv.cn

[D04] 删除元素
来源：http://tfn.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xib.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cjl.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yye.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://lgg.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://snf.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://azm.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zim.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://que.hnqzz.top

[D05] 访问与修改元素
来源：http://tzg.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vzw.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xdg.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xqo.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://mrj.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://qbl.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://ajv.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofc.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xku.hywenlv.cn

[D06] 数组长度
来源：http://vss.xylfe.cn

Py:   len(arr)
来源：http://qgv.cheryme.top

PHP:  count($arr);
来源：http://arx.hnqzz.top

JS:   arr.length
来源：http://jdl.nwbrower.top

TS:   arr.length
来源：http://hip.fanxiaobao.xyz

Java: list.size();
来源：http://pnh.guannengcc.top

Go:   len(arr)
来源：http://wrg.tarul.cn

Ruby: arr.length; arr.size
来源：http://hwa.xziqi.cn

C#:   list.Count;
来源：http://jnl.sxryk.cn

[D07] 切片 / 取子数组
来源：http://rjp.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qrh.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ppp.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://gku.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://opy.shuidangran.top

Java: list.subList(1, 4);
来源：http://gpw.yueranfly.top

Go:   arr[1:4]
来源：http://jkl.zycfv.cn

Ruby: arr[1, 3]
来源：http://gpl.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://ikm.quarkkingdee.top

[D08] 合并两个数组
来源：http://rdk.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://bvi.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://mor.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vzw.jqgfzy.top

TS:   [...a, ...b];
来源：http://yyh.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ghy.yonumen.top

Go:   append(a, b...)
来源：http://orp.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://xfr.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://ftj.yj20258.top

[D09] 排序（升序）
来源：http://svi.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://bli.zhijiandao.cn

PHP:  sort($arr);
来源：http://bsi.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wyn.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kou.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vdy.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jrq.yueranfly.top

Ruby: arr.sort
来源：http://ifg.yongpay.top

C#:   list.Sort();
来源：http://vpb.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ojw.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rze.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujc.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zio.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvx.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://las.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://day.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://asc.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://unw.sufxvd.cn

[D11] 反转数组
来源：http://qpv.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://iqt.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://pki.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ndt.xziqi.cn

TS:   [...arr].reverse();
来源：http://isl.jyoumei.cn

Java: Collections.reverse(list);
来源：http://cbk.pycfn.com

Go:   slices.Reverse(arr)
来源：http://iej.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://fhx.zdbjq.cn

C#:   list.Reverse();
来源：http://zbs.uphjek.com

[D12] 查找元素下标
来源：http://zaa.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://ugu.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://won.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hzg.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqd.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ewq.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://daq.xuanzx.com

Ruby: arr.index(x)
来源：http://oze.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://tmd.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://fzs.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gsg.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ufq.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://phc.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://zph.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ent.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://btc.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yqo.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bgl.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://ion.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwd.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lmo.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://qzl.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://hwe.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fwi.jinghuilouyu.cn

Go:   // 手写循环
来源：http://vdd.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://iwk.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ica.daria6918.cn

[D15] 去重
来源：http://ewi.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vkc.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://vrh.bbcook.cn

JS:   [...new Set(arr)]
来源：http://dmp.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://ekv.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qhb.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tzf.jqgufenzy.top

Ruby: arr.uniq
来源：http://xxs.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://drk.yongpay.top

[D16] 求和与平均值
来源：http://ono.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nnr.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://len.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qhv.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmy.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xac.hnxiangtu.top

Go:   // 手写循环累加
来源：http://ntv.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zho.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://nqv.yj20258888.top

[D17] 最大值与最小值
来源：http://fma.birdmap.top

Py:   max(arr);  min(arr)
来源：http://cmh.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://uks.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qlq.yj20258888.top

TS:   Math.max(...arr);
来源：http://wmo.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://qxl.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gkn.ivvv.top

Ruby: arr.max;  arr.min
来源：http://ezv.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://ant.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://exf.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nzt.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://hdi.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yln.gzhubu.top

TS:   nested.flat();
来源：http://bxh.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://euo.aizwys.cn

Go:   // 手写双层循环
来源：http://sra.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://jyz.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ega.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://kim.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ymj.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ess.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dcj.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nws.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cta.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://oxo.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://uzp.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cua.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://ufn.pycfn.com

Py:   Counter(arr)
来源：http://gzj.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://nlp.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pqf.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://son.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://txb.daria6918.cn

Go:   // 手写 map[T]int
来源：http://qmn.cashguo.top

Ruby: arr.tally
来源：http://emy.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axs.cashguo.top

[D21] 判断是否包含某元素
来源：http://ddl.redwolf501.top

Py:   x in arr
来源：http://igi.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://ggp.cashguo.top

JS:   arr.includes(x)
来源：http://ukx.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://hko.yangfankeji.com

Java: list.contains(x)
来源：http://ids.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://sgv.yuanzhike.top

Ruby: arr.include?(x)
来源：http://tep.zhongyouzk.top

C#:   list.Contains(x)
来源：http://zab.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://osf.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nux.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mil.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://djv.chenjidiqi.icu

TS:   [...arr];
来源：http://owp.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://kjs.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://oao.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://anb.hnqzz.top

C#:   new List<int>(list);
来源：http://ylc.gaohongyu789.top

[D23] reduce 累积计算
来源：http://wfs.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zja.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxw.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kgg.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ngc.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mxt.zdqjudy.top

Go:   // 手写循环
来源：http://fgz.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hcr.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dgl.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://kdu.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://geg.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://woa.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dch.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zqe.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tdl.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tsj.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mql.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ska.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://luy.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://drc.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lct.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://plf.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lof.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oil.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rdn.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nfa.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pfi.zycfv.cn

[D26] 数组转字符串
来源：http://ctt.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://cfe.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://eoj.mhx1999.top

JS:   arr.join(", ")
来源：http://fvz.andypj.xyz

TS:   arr.join(", ")
来源：http://kqw.redwolf501.top

Java: String.join(", ", list)
来源：http://vwp.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://bky.bjfxy.top

Ruby: arr.join(", ")
来源：http://wdc.cheryme.top

C#:   string.Join(", ", list)
来源：http://dpy.chenjidiqi.icu

================================================================================
来源：http://mzt.hongshengwenyu.top

E. 字符串处理
来源：http://oqr.jinqigufen.top

================================================================================
来源：http://qzn.hfpthk.cn

[E01] 拼接字符串
来源：http://gws.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zzd.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oae.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzq.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hby.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://myd.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ncn.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ndq.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vee.ctjpmb.com

[E02] 重复字符串
来源：http://nyh.tarul.cn

Py:   "ab" * 3
来源：http://kfn.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://imr.yuxming.cn

JS:   "ab".repeat(3)
来源：http://uel.jianghu66.top

TS:   "ab".repeat(3)
来源：http://iyb.zhengqikj.top

Java: "ab".repeat(3)
来源：http://kyl.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://vug.nanxuanxn.top

Ruby: "ab" * 3
来源：http://ncs.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://poj.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://gni.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://siz.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kpc.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eip.cashguo.top

TS:   s.slice(1, 4)
来源：http://xic.ctjpmb.com

Java: s.substring(1, 4)
来源：http://jsu.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qdl.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://imr.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://jqq.xuanzx.com

[E04] 查找子串位置
来源：http://kui.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://spr.tanke756.top

PHP:  strpos($s, "x");
来源：http://enq.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gzw.wangdashe.top

TS:   s.indexOf("x")
来源：http://uec.zhoulong.xyz

Java: s.indexOf("x")
来源：http://ejj.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://cnu.nwbrower.top

Ruby: s.index("x")
来源：http://jev.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://ubv.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lkr.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://unf.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kvg.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ort.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uci.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucw.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dmg.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ext.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jai.sysykeji.top

[E06] 替换子串
来源：http://yaq.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kyt.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://roh.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lce.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://omd.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mom.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://csh.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zcf.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://mvy.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://mdn.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oqb.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vke.yonumen.top


<!-- 参考信息 -->