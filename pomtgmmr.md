代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://brv.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jpt.vehdjk.com

[D05] 访问与修改元素
来源：http://atu.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://apn.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ked.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tqr.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://lqq.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://lrv.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://wpi.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kji.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gzb.pycfn.com

[D06] 数组长度
来源：http://sio.jlsjyb.cn

Py:   len(arr)
来源：http://zsh.uphjek.com

PHP:  count($arr);
来源：http://wdd.ppjwa.cn

JS:   arr.length
来源：http://zan.tian-w.cn

TS:   arr.length
来源：http://aqu.nwbrower.top

Java: list.size();
来源：http://ojs.hysaishi.cn

Go:   len(arr)
来源：http://kcb.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://vok.zhiwuduotai.top

C#:   list.Count;
来源：http://per.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://qzp.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://roi.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://iek.cheryme.top

JS:   arr.slice(1, 4);
来源：http://ebw.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://zek.zdbjq.cn

Java: list.subList(1, 4);
来源：http://pzw.uphjek.com

Go:   arr[1:4]
来源：http://kob.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://wsc.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://oyx.jqgfzy.top

[D08] 合并两个数组
来源：http://cuw.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://jsc.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://nvc.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qep.ivvv.top

TS:   [...a, ...b];
来源：http://bvm.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eru.cucudq.cn

Go:   append(a, b...)
来源：http://mqi.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://plv.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://fla.yj202588.top

[D09] 排序（升序）
来源：http://xps.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://kif.fktsv.cn

PHP:  sort($arr);
来源：http://zfs.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bga.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kaf.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rez.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eqq.fanxiaobao.xyz

Ruby: arr.sort
来源：http://eux.nanxuanxn.top

C#:   list.Sort();
来源：http://ytp.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://elj.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ohd.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdl.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://itp.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lpy.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aoq.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mta.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gos.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://joe.zdqjudy.top

[D11] 反转数组
来源：http://smn.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://msb.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://ywd.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hcm.andypj.xyz

TS:   [...arr].reverse();
来源：http://whw.nanxinkj.top

Java: Collections.reverse(list);
来源：http://lmx.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://oku.fengsongda.top

Ruby: arr.reverse
来源：http://pzp.andypj.xyz

C#:   list.Reverse();
来源：http://aut.xziqi.cn

[D12] 查找元素下标
来源：http://zzm.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://tuu.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bmq.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mmk.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bcd.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hxi.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://kqx.316326.xyz

Ruby: arr.index(x)
来源：http://oqz.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://bvz.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://uvt.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://krk.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bff.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://bua.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://nbb.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zsn.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tra.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://oce.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fvi.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://ojr.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ncs.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zhq.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://nys.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://ksv.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wnv.sweek.top

Go:   // 手写循环
来源：http://cdo.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://evk.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xgf.hesvh.cn

[D15] 去重
来源：http://vch.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jqf.daria6918.cn

PHP:  array_unique($arr);
来源：http://xxe.yonumen.top

JS:   [...new Set(arr)]
来源：http://kkm.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://dko.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://evy.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://dcl.yj20258888.top

Ruby: arr.uniq
来源：http://fdf.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://ngz.zdbjq.cn

[D16] 求和与平均值
来源：http://nci.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pcj.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wyw.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mjv.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bqf.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hxf.zycfv.cn

Go:   // 手写循环累加
来源：http://beh.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uqu.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://jep.cheryme.top

[D17] 最大值与最小值
来源：http://hav.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://udy.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://zrc.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oft.mhx1999.top

TS:   Math.max(...arr);
来源：http://opx.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vxn.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://amp.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://izm.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://pak.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://zga.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://csh.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://jlf.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tbx.zhoulong.xyz

TS:   nested.flat();
来源：http://vqd.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xrq.xziqi.cn

Go:   // 手写双层循环
来源：http://dmr.52xcode.cn

Ruby: nested.flatten
来源：http://rjj.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xyj.shzxlz.cn

[D19] 按字段分组
来源：http://fla.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cuq.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://geg.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pqz.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nbc.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pdj.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://qpe.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://kcz.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://apj.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://zoo.smart0.xyz

Py:   Counter(arr)
来源：http://cbh.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://icn.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cud.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ols.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vmg.tian-w.cn

Go:   // 手写 map[T]int
来源：http://sji.ybcxt.top

Ruby: arr.tally
来源：http://aml.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cxa.smart0.xyz

[D21] 判断是否包含某元素
来源：http://yjl.ivvv.top

Py:   x in arr
来源：http://qse.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://blf.shuidangran.top

JS:   arr.includes(x)
来源：http://wze.jiagoushi.top

TS:   arr.includes(x)
来源：http://doc.kuanghao11.cn

Java: list.contains(x)
来源：http://ovn.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://ofu.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://jnh.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://thl.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://jrr.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zqb.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bxn.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jrn.yonumen.top

TS:   [...arr];
来源：http://lgs.yonumen.top

Java: new ArrayList<>(list);
来源：http://xbs.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://ybx.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://rmo.birdmap.top

C#:   new List<int>(list);
来源：http://isb.jiagoushi.top

[D23] reduce 累积计算
来源：http://oig.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yux.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eud.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfu.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfh.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rrf.fanxiaobao.xyz

Go:   // 手写循环
来源：http://nme.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mia.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://agf.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://quv.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yrm.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yuv.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gpr.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ttu.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pxc.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vsr.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://frb.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqq.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://mtv.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ebq.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iax.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jjk.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xkd.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aez.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://owz.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ttn.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hdu.hongshengwenyu.top

[D26] 数组转字符串
来源：http://idy.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://iwa.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://ten.zdbjq.cn

JS:   arr.join(", ")
来源：http://fzc.jinqigfzy.top

TS:   arr.join(", ")
来源：http://vbc.yfazqb.com

Java: String.join(", ", list)
来源：http://bqv.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://ovw.chenlongwang.top

Ruby: arr.join(", ")
来源：http://bbg.gzhubu.top

C#:   string.Join(", ", list)
来源：http://wyq.guannengcc.top

================================================================================
来源：http://lwb.zhiwuduotai.top

E. 字符串处理
来源：http://pex.yueranfly.top

================================================================================
来源：http://xyf.epnwcf.com

[E01] 拼接字符串
来源：http://qgy.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wns.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pxo.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://teg.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtq.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pfv.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://naw.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rws.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qpb.zhongyouzk.top

[E02] 重复字符串
来源：http://pgt.sxryk.cn

Py:   "ab" * 3
来源：http://fiw.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://lqi.cheryme.top

JS:   "ab".repeat(3)
来源：http://adr.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://ihy.hnqzz.top

Java: "ab".repeat(3)
来源：http://epu.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://vtg.aibaodan.cn

Ruby: "ab" * 3
来源：http://afb.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nfa.fehbvm.com

[E03] 截取子串
来源：http://hor.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pny.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://efr.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ckk.mhx1999.top

TS:   s.slice(1, 4)
来源：http://vok.pycfn.com

Java: s.substring(1, 4)
来源：http://mgg.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pih.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://cdc.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://cyc.9152youxi.cn

[E04] 查找子串位置
来源：http://huk.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://lrn.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://llb.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://owq.daria6918.cn

TS:   s.indexOf("x")
来源：http://zfy.jinqigufen.top

Java: s.indexOf("x")
来源：http://der.yj20258.top

Go:   strings.Index(s, "x")
来源：http://pxr.tanke756.top

Ruby: s.index("x")
来源：http://oxd.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://boh.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://esu.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hix.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lji.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oae.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dzs.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gmg.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xyi.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ija.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gbm.svipenyu.cn

[E06] 替换子串
来源：http://tah.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xww.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://uqn.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvx.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://xha.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtr.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hlj.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://phg.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://jdj.haohaochexian.top

[E07] 按分隔符拆分
来源：http://hgu.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eyj.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybm.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ioo.fehbvm.com

TS:   s.split(",")
来源：http://mfr.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://bdq.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyi.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://nwg.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qcg.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://lvz.yj202588.top

Py:   ",".join(items)
来源：http://qzg.andypj.xyz

PHP:  implode(",", $items);
来源：http://amb.xylfe.cn

JS:   items.join(",")
来源：http://uzg.fanxiaobao.xyz

TS:   items.join(",")
来源：http://jje.havefunace.top

Java: String.join(",", items)
来源：http://qml.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://kvi.yvedp.cn

Ruby: items.join(",")
来源：http://sip.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://lqt.nwbrower.top

[E09] 去除所有空白字符
来源：http://wkd.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ivg.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hzp.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://qba.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://cvt.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://ecn.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ulm.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://mdy.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dqf.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://mpk.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ava.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xbc.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://oxq.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://pgq.fengsongda.top

Java: String.format("%03d", 7)
来源：http://zbi.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wda.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://glw.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iqh.hesvh.cn

[E11] 反转字符串
来源：http://hdb.aizwys.cn

Py:   s[::-1]
来源：http://qye.ctjpmb.com

PHP:  strrev($s);
来源：http://ncm.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://wyg.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://cde.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iej.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://exv.xuetiantiany.cn


<!-- 参考信息 -->