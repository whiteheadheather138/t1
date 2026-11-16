代发 wailian999

[D03] 在指定位置插入元素
来源：http://clm.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://dec.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dyk.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pui.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://tpv.hysaishi.cn

Java: list.add(0, 0);
来源：http://omj.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://rdd.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xna.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://oaj.zhengqikj.top

[D04] 删除元素
来源：http://prw.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rvs.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pjv.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://epq.yj20258.top

TS:   arr.splice(0, 1);
来源：http://lbo.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nek.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjz.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yrb.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lty.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://bjc.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nbe.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dul.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mcm.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://xmv.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://otj.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://uxr.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjf.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ycf.feifeiyinyue.top

[D06] 数组长度
来源：http://ora.snrcjt.cn

Py:   len(arr)
来源：http://lbo.yuanzhike.top

PHP:  count($arr);
来源：http://xty.nwbrower.top

JS:   arr.length
来源：http://wvk.shangyingyoupin.top

TS:   arr.length
来源：http://rfy.snrcjt.cn

Java: list.size();
来源：http://xkg.vqdsnc.cn

Go:   len(arr)
来源：http://vbb.meibo888.top

Ruby: arr.length; arr.size
来源：http://cuf.mhx1999.top

C#:   list.Count;
来源：http://vcg.sysykeji.top

[D07] 切片 / 取子数组
来源：http://ceh.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://woo.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://oqa.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://ozd.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://mjy.redwolf501.top

Java: list.subList(1, 4);
来源：http://uwu.nanxuanxn.top

Go:   arr[1:4]
来源：http://pvv.zycfv.cn

Ruby: arr[1, 3]
来源：http://ewe.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://kpf.zycfv.cn

[D08] 合并两个数组
来源：http://sbm.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://ybp.meibo888.top

PHP:  array_merge($a, $b);
来源：http://dhp.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tjs.yj202588.top

TS:   [...a, ...b];
来源：http://ifl.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ips.mhx1999.top

Go:   append(a, b...)
来源：http://mzx.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://ogm.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://rtx.tanke756.top

[D09] 排序（升序）
来源：http://vuh.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://agg.zhoulong.xyz

PHP:  sort($arr);
来源：http://bjg.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pxj.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wad.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eoe.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jnu.andypj.xyz

Ruby: arr.sort
来源：http://rhs.mhx1999.top

C#:   list.Sort();
来源：http://dxz.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hvc.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jwi.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qmx.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwg.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lau.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzn.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ujz.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ath.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tgm.zhoulong.xyz

[D11] 反转数组
来源：http://fxn.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://xix.bjfxy.top

PHP:  array_reverse($arr);
来源：http://vph.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxv.yongpay.top

TS:   [...arr].reverse();
来源：http://zag.hesvh.cn

Java: Collections.reverse(list);
来源：http://hpf.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://gyo.feifeiyinyue.top

Ruby: arr.reverse
来源：http://fsj.cucudq.cn

C#:   list.Reverse();
来源：http://wzd.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://ouu.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://dzd.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vxp.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yps.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nto.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mse.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://hhi.zhengqikj.top

Ruby: arr.index(x)
来源：http://qby.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://fni.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://ocm.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gxm.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rby.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://wuv.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://zjc.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vlr.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kwe.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wak.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dho.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://xiw.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nex.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jhc.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://dsi.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://bfp.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sua.sysykeji.top

Go:   // 手写循环
来源：http://dju.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://txx.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hoz.guowangkeji.top

[D15] 去重
来源：http://rrd.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hpg.hcnkem.com

PHP:  array_unique($arr);
来源：http://vzc.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://fgp.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://xmw.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wth.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zuz.jqgufenzy.top

Ruby: arr.uniq
来源：http://sxv.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://tlp.zdbjq.cn

[D16] 求和与平均值
来源：http://rnx.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uin.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nbo.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://phe.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dsq.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yqj.0kj1m.cn

Go:   // 手写循环累加
来源：http://gya.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://icy.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://zar.yj202588.top

[D17] 最大值与最小值
来源：http://hcf.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://fyp.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://pzk.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yxj.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://igj.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vjn.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://psj.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://ojh.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://cax.yongpay.top

[D18] 扁平化嵌套数组
来源：http://lrq.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://elt.meibo888.top

PHP:  array_merge(...$nested);
来源：http://ihz.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ycg.zhixingplan.top

TS:   nested.flat();
来源：http://rcj.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kkg.yangfankeji.com

Go:   // 手写双层循环
来源：http://qet.zhoulong.xyz

Ruby: nested.flatten
来源：http://kqw.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gqc.yongpay.top

[D19] 按字段分组
来源：http://jhl.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://doa.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qbq.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uld.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rqq.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oaw.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://gap.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bqy.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zjq.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://xae.dashuyun.cn

Py:   Counter(arr)
来源：http://vsi.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://blb.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aji.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ioy.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ijh.daria6918.cn

Go:   // 手写 map[T]int
来源：http://xtr.jlsjyb.cn

Ruby: arr.tally
来源：http://jze.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://szi.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://iys.hammf.cn

Py:   x in arr
来源：http://xyt.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://gtg.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://wan.hnxiangtu.top

TS:   arr.includes(x)
来源：http://lui.gogol.net.cn

Java: list.contains(x)
来源：http://ori.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://bey.fktsv.cn

Ruby: arr.include?(x)
来源：http://myi.zhijiandao.cn

C#:   list.Contains(x)
来源：http://hke.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://nlw.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hki.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evo.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kje.yongpay.top

TS:   [...arr];
来源：http://gke.tanke756.top

Java: new ArrayList<>(list);
来源：http://ehd.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cwt.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://ujf.jyoumei.cn

C#:   new List<int>(list);
来源：http://rcz.zhongyouzk.top

[D23] reduce 累积计算
来源：http://oen.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ozj.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tbg.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfd.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ijm.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bxh.jyoumei.cn

Go:   // 手写循环
来源：http://jjx.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pee.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bbq.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://gkj.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mkm.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bsa.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bur.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lru.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yjd.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogk.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://awi.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pzl.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://wtq.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vwg.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwz.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wwp.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pvh.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mig.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mws.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qmv.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ibi.chenjidiqi.icu

[D26] 数组转字符串
来源：http://phy.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://msk.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://xko.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://xme.mhx1999.top

TS:   arr.join(", ")
来源：http://wwf.yangfankeji.com

Java: String.join(", ", list)
来源：http://ahe.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://zwi.52xcode.cn

Ruby: arr.join(", ")
来源：http://gwn.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://yzg.hfpthk.cn

================================================================================
来源：http://qsp.sufxvd.cn

E. 字符串处理
来源：http://sbt.jianghu66.top

================================================================================
来源：http://tmk.316326.xyz

[E01] 拼接字符串
来源：http://ejb.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ift.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jng.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mwe.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zqv.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zbk.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://phm.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tmw.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dfn.pycfn.com

[E02] 重复字符串
来源：http://vur.ivvv.top

Py:   "ab" * 3
来源：http://paj.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://wqo.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://cxa.hammf.cn

TS:   "ab".repeat(3)
来源：http://vfx.cucudq.cn

Java: "ab".repeat(3)
来源：http://ibw.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://pgb.9152youxi.cn

Ruby: "ab" * 3
来源：http://qwr.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wxc.bjfxy.top

[E03] 截取子串
来源：http://qhe.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vyi.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lly.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gwu.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://tyc.guannengcc.top

Java: s.substring(1, 4)
来源：http://xfr.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egs.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://wzd.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://plm.cashguo.top

[E04] 查找子串位置
来源：http://dnl.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://xwn.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://owf.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://icb.tarul.cn

TS:   s.indexOf("x")
来源：http://vij.sufxvd.cn

Java: s.indexOf("x")
来源：http://vnq.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://pyy.tarul.cn

Ruby: s.index("x")
来源：http://zcc.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://nfs.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ncn.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fcy.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eoh.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjk.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wft.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fsj.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vcb.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://huw.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kjp.dashuyun.cn

[E06] 替换子串
来源：http://cks.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wkt.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://pla.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uij.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://aqt.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gvs.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tqj.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uax.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://rxy.9152youxi.cn

[E07] 按分隔符拆分
来源：http://qdq.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyh.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eiv.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbx.dianchejie.cn

TS:   s.split(",")
来源：http://fnz.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://opl.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uur.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://xrv.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oyj.jianghu66.top

[E08] 数组按分隔符合并
来源：http://blq.ehwqpu.com

Py:   ",".join(items)
来源：http://kjq.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://efg.shangyingyoupin.top

JS:   items.join(",")
来源：http://ljg.quarkkingdee.top

TS:   items.join(",")
来源：http://mjn.meibo888.top

Java: String.join(",", items)
来源：http://qof.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://mzf.yangfankeji.com

Ruby: items.join(",")
来源：http://hln.cashguo.top

C#:   string.Join(",", items)
来源：http://ivf.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://vbg.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sgd.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aik.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://ncf.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://hiz.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://tki.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kvw.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://kvc.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gmf.fzhhl.top


<!-- 参考信息 -->