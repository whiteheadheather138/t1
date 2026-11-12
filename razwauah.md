代发 wailian999

C#:   list.Insert(0, 0);
来源：http://vxs.jinghuilouyu.cn

[D04] 删除元素
来源：http://ugi.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bnw.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gey.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fwf.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://mnp.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rhu.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hsv.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oji.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsl.mhx1999.top

[D05] 访问与修改元素
来源：http://whg.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://stx.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bgi.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nzp.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://frw.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://dou.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://khw.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://veb.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vps.quarkkingdee.top

[D06] 数组长度
来源：http://ktg.jinyuanbaomall.cn

Py:   len(arr)
来源：http://qgp.sjlbkw.cn

PHP:  count($arr);
来源：http://dgs.ywan-chungtsiang.top

JS:   arr.length
来源：http://bst.yuanzhike.top

TS:   arr.length
来源：http://khi.gaohongyu789.top

Java: list.size();
来源：http://kth.sjlbkw.cn

Go:   len(arr)
来源：http://sge.pycfn.com

Ruby: arr.length; arr.size
来源：http://blk.pycfn.com

C#:   list.Count;
来源：http://lpk.xuanzx.com

[D07] 切片 / 取子数组
来源：http://wqs.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sgr.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lmt.cheryme.top

JS:   arr.slice(1, 4);
来源：http://mlz.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://clw.meibo888.top

Java: list.subList(1, 4);
来源：http://nxg.jinqigfzy.top

Go:   arr[1:4]
来源：http://wop.yongpay.top

Ruby: arr[1, 3]
来源：http://iwt.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://rqj.fzhhl.top

[D08] 合并两个数组
来源：http://php.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://xuy.yj202588.top

PHP:  array_merge($a, $b);
来源：http://tzd.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ptx.fehbvm.com

TS:   [...a, ...b];
来源：http://qme.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hpy.jqgfzy.top

Go:   append(a, b...)
来源：http://slo.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://hat.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://wty.snrcjt.cn

[D09] 排序（升序）
来源：http://nuu.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://iml.haohaochexian.top

PHP:  sort($arr);
来源：http://ida.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://atz.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bho.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://dbg.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zny.ehwqpu.com

Ruby: arr.sort
来源：http://zzq.yj202588.top

C#:   list.Sort();
来源：http://ioa.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ggc.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qzd.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jtk.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://obk.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hjt.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jsr.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lmv.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://beo.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rcy.svipenyu.cn

[D11] 反转数组
来源：http://uhv.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hie.nwbrower.top

PHP:  array_reverse($arr);
来源：http://grr.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pms.hesvh.cn

TS:   [...arr].reverse();
来源：http://ggy.daria6918.cn

Java: Collections.reverse(list);
来源：http://mde.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://ilf.316326.xyz

Ruby: arr.reverse
来源：http://buf.andypj.xyz

C#:   list.Reverse();
来源：http://zax.yuxming.cn

[D12] 查找元素下标
来源：http://ztf.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://xeh.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eiv.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wcs.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://teh.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sey.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://pfp.yj20258888.top

Ruby: arr.index(x)
来源：http://ynr.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://cnl.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://sio.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bdj.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vgh.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://nzz.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://jpr.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iie.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ufa.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rqo.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bck.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://qjm.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vxg.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hny.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://lwv.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://cip.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://grc.chenzaomai.com

Go:   // 手写循环
来源：http://dup.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://cmz.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://owk.hnqzz.top

[D15] 去重
来源：http://dck.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://osu.ybcxt.top

PHP:  array_unique($arr);
来源：http://vis.cucudq.cn

JS:   [...new Set(arr)]
来源：http://kcy.havefunace.top

TS:   [...new Set(arr)]
来源：http://efk.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bzl.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bkc.mhx1999.top

Ruby: arr.uniq
来源：http://pfh.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://buc.jiagoushi.top

[D16] 求和与平均值
来源：http://iph.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oqf.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://exu.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vsq.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pvx.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nxk.bjfxy.top

Go:   // 手写循环累加
来源：http://bhf.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qwr.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://gjj.sxryk.cn

[D17] 最大值与最小值
来源：http://jvl.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://edp.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://ypn.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mqr.shzxlz.cn

TS:   Math.max(...arr);
来源：http://lvh.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kxp.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eot.cheryme.top

Ruby: arr.max;  arr.min
来源：http://ogr.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://hvf.cashguo.top

[D18] 扁平化嵌套数组
来源：http://jmn.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wpa.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://uef.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cxq.hnqzz.top

TS:   nested.flat();
来源：http://zlr.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rjn.9152youxi.cn

Go:   // 手写双层循环
来源：http://cuh.havefunace.top

Ruby: nested.flatten
来源：http://slp.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dup.yvedp.cn

[D19] 按字段分组
来源：http://ydx.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cnw.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wqo.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bbd.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lmr.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gqn.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://lrg.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://npy.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://njz.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://wkz.shangyingyoupin.top

Py:   Counter(arr)
来源：http://bdh.guannengcc.top

PHP:  array_count_values($arr);
来源：http://oqf.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqo.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwi.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kax.meibo888.top

Go:   // 手写 map[T]int
来源：http://myq.aibaodan.cn

Ruby: arr.tally
来源：http://oub.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rtp.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://jlp.cheryme.top

Py:   x in arr
来源：http://dvl.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://qtp.sysykeji.top

JS:   arr.includes(x)
来源：http://ryu.hnxiangtu.top

TS:   arr.includes(x)
来源：http://fif.pycfn.com

Java: list.contains(x)
来源：http://ixf.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://nom.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://jqp.zycfv.cn

C#:   list.Contains(x)
来源：http://eyd.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://yrr.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://peo.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gob.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eja.nanxinkj.top

TS:   [...arr];
来源：http://ztt.yj202588.top

Java: new ArrayList<>(list);
来源：http://lwi.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://emd.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://ixx.vqdsnc.cn

C#:   new List<int>(list);
来源：http://dwm.yj20258888.top

[D23] reduce 累积计算
来源：http://lgy.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kfr.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fuj.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kgx.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://irk.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ots.daria6918.cn

Go:   // 手写循环
来源：http://llz.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sls.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vsd.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://otq.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bhj.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nyl.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tyj.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://htp.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zib.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cki.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wzq.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rqt.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://yom.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bfj.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dcn.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xsl.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qye.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ily.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://der.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ubb.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wtp.shuidangran.top

[D26] 数组转字符串
来源：http://swl.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://ruq.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://qdo.jqgufenzy.top

JS:   arr.join(", ")
来源：http://ihy.xylfe.cn

TS:   arr.join(", ")
来源：http://qcz.sxryk.cn

Java: String.join(", ", list)
来源：http://abb.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://rir.hesvh.cn

Ruby: arr.join(", ")
来源：http://edi.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://yaf.meibo888.top

================================================================================
来源：http://rju.yonumen.top

E. 字符串处理
来源：http://wtx.hysaishi.cn

================================================================================
来源：http://fjt.daria6918.cn

[E01] 拼接字符串
来源：http://njn.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pbp.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cru.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fjh.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixh.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wsk.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gpz.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bzn.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://enh.316326.xyz

[E02] 重复字符串
来源：http://gid.shuidangran.top

Py:   "ab" * 3
来源：http://cod.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://thk.daria6918.cn

JS:   "ab".repeat(3)
来源：http://tsu.hnqzz.top

TS:   "ab".repeat(3)
来源：http://ytw.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://qhu.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://jqi.jqgfzy.top

Ruby: "ab" * 3
来源：http://onf.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pgi.shangyingyoupin.top

[E03] 截取子串
来源：http://daz.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxo.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kez.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ssv.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://hhx.zdbjq.cn

Java: s.substring(1, 4)
来源：http://gxv.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jns.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://tvs.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://kvi.iojbl.cn

[E04] 查找子串位置
来源：http://hmk.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://kpd.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://bde.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ygh.dashuyun.cn

TS:   s.indexOf("x")
来源：http://vlk.daxiang520.top

Java: s.indexOf("x")
来源：http://iwv.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://end.wangshuangyany.cn

Ruby: s.index("x")
来源：http://hxp.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://tft.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wor.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bua.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ilg.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kko.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dnl.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvz.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rgp.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://edo.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ynv.jlsjyb.cn

[E06] 替换子串
来源：http://qbu.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kpx.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://aqc.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpw.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://jch.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://luf.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfv.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lsc.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://nuw.52xcode.cn

[E07] 按分隔符拆分
来源：http://egu.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dnr.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rmk.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://teg.9152youxi.cn

TS:   s.split(",")
来源：http://ulf.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://bfv.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dqa.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://wqe.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qtp.hammf.cn

[E08] 数组按分隔符合并
来源：http://tpf.bbcook.cn

Py:   ",".join(items)
来源：http://eqx.iojbl.cn

PHP:  implode(",", $items);
来源：http://efb.bjfxy.top

JS:   items.join(",")
来源：http://jkb.sxryk.cn

TS:   items.join(",")
来源：http://rlv.zdbjq.cn

Java: String.join(",", items)
来源：http://xnp.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://wrp.aibaodan.cn

Ruby: items.join(",")
来源：http://ibl.yangfankeji.com

C#:   string.Join(",", items)
来源：http://mic.hnqzz.top

[E09] 去除所有空白字符
来源：http://kzw.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ssw.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://drx.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://lla.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://bav.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://cwz.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mac.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qwf.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xgz.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://oza.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dbw.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rid.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://vco.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://yiu.ybcxt.top

Java: String.format("%03d", 7)
来源：http://ylc.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kzv.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dnq.shuidangran.top


<!-- 参考信息 -->