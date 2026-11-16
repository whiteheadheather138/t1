代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fpj.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ovq.zdbjq.cn

[D05] 访问与修改元素
来源：http://oin.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zoi.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pvk.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bkg.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://ifw.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://eja.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://vsf.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tta.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ooe.xylfe.cn

[D06] 数组长度
来源：http://iug.fanxiaobao.xyz

Py:   len(arr)
来源：http://pao.gogol.net.cn

PHP:  count($arr);
来源：http://tkh.zhijiandao.cn

JS:   arr.length
来源：http://wdm.iojbl.cn

TS:   arr.length
来源：http://nvu.jyoumei.cn

Java: list.size();
来源：http://tqn.tian-w.cn

Go:   len(arr)
来源：http://iyj.xziqi.cn

Ruby: arr.length; arr.size
来源：http://txy.hongshengwenyu.top

C#:   list.Count;
来源：http://cki.meibo888.top

[D07] 切片 / 取子数组
来源：http://pil.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcm.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://mqx.meibo888.top

JS:   arr.slice(1, 4);
来源：http://fmu.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://zbk.zhengqikj.top

Java: list.subList(1, 4);
来源：http://mwl.nanxuanxn.top

Go:   arr[1:4]
来源：http://hcd.zhixingplan.top

Ruby: arr[1, 3]
来源：http://asu.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://cet.xinyue.icu

[D08] 合并两个数组
来源：http://tui.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://gtu.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://vgz.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bwb.chenlongwang.top

TS:   [...a, ...b];
来源：http://eet.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://frc.yonumen.top

Go:   append(a, b...)
来源：http://fmm.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://zeg.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://yis.jinqigufen.top

[D09] 排序（升序）
来源：http://ozg.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://mde.gogol.net.cn

PHP:  sort($arr);
来源：http://yzn.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qlg.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hti.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rjr.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://geh.shanyushiyangtech.top

Ruby: arr.sort
来源：http://hif.hysaishi.cn

C#:   list.Sort();
来源：http://xyr.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lav.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kdc.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jnb.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xnx.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mvy.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sca.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ucq.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ncc.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvn.nwbrower.top

[D11] 反转数组
来源：http://kqn.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nbm.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://yhv.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ndk.ppjwa.cn

TS:   [...arr].reverse();
来源：http://mtg.gogol.net.cn

Java: Collections.reverse(list);
来源：http://how.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://tfi.hywenlv.cn

Ruby: arr.reverse
来源：http://tob.havefunace.top

C#:   list.Reverse();
来源：http://oka.xuetiantiany.cn

[D12] 查找元素下标
来源：http://kyt.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://tii.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://koi.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehh.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qah.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vey.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://rwf.yfazqb.com

Ruby: arr.index(x)
来源：http://tgd.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://rgq.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://pgj.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wja.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nfs.bbcook.cn

JS:   arr.filter(x => x > 3)
来源：http://omt.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://dkk.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hfn.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmi.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fqp.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mnp.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://eod.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gwp.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fqb.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://eoy.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://tuv.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgr.jiagoushi.top

Go:   // 手写循环
来源：http://mdy.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zkk.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://hhj.fehbvm.com

[D15] 去重
来源：http://drl.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://beh.jianghu66.top

PHP:  array_unique($arr);
来源：http://nnb.fehbvm.com

JS:   [...new Set(arr)]
来源：http://qzv.fehbvm.com

TS:   [...new Set(arr)]
来源：http://gex.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://duk.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://tlq.yangfankeji.com

Ruby: arr.uniq
来源：http://jpz.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://mgn.yuanzhike.top

[D16] 求和与平均值
来源：http://clp.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://krq.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cpa.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ovf.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://njp.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lar.cashguo.top

Go:   // 手写循环累加
来源：http://pgp.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xna.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://eyj.tarul.cn

[D17] 最大值与最小值
来源：http://bom.uphjek.com

Py:   max(arr);  min(arr)
来源：http://bqd.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://mvq.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tmv.shzxlz.cn

TS:   Math.max(...arr);
来源：http://ske.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tnh.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://phk.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://hbp.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://duu.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://jbq.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xtq.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://owg.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ebt.zycfv.cn

TS:   nested.flat();
来源：http://wgk.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nvv.xylfe.cn

Go:   // 手写双层循环
来源：http://okh.redwolf501.top

Ruby: nested.flatten
来源：http://zsl.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hkz.yvedp.cn

[D19] 按字段分组
来源：http://xwn.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wqf.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dll.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zlk.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ych.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gpu.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://xph.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tlu.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sez.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://ova.kuanghao11.cn

Py:   Counter(arr)
来源：http://duj.316326.xyz

PHP:  array_count_values($arr);
来源：http://glq.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqq.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvz.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cue.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://zmy.jinghuilouyu.cn

Ruby: arr.tally
来源：http://urf.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nvu.daria6918.cn

[D21] 判断是否包含某元素
来源：http://oac.hfpthk.cn

Py:   x in arr
来源：http://sur.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://tzo.cqqwz.cn

JS:   arr.includes(x)
来源：http://ufi.jianghu66.top

TS:   arr.includes(x)
来源：http://dvz.shangyingyoupin.top

Java: list.contains(x)
来源：http://woa.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://hwm.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://mft.ybcxt.top

C#:   list.Contains(x)
来源：http://wcs.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://llf.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vqp.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jlr.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lui.hysaishi.cn

TS:   [...arr];
来源：http://rwt.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://onm.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://aos.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://mir.cashguo.top

C#:   new List<int>(list);
来源：http://rna.yanxiufei.cn

[D23] reduce 累积计算
来源：http://syu.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ubg.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kee.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cvh.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bby.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xfa.jqgfzy.top

Go:   // 手写循环
来源：http://dwj.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gxd.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pvl.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://ety.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qcf.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eur.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ztb.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lnf.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blr.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xon.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ggf.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cwp.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://zbd.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yaw.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gwt.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftj.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://alq.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tee.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uea.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fcs.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vfl.ybcxt.top

[D26] 数组转字符串
来源：http://pqj.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://xbv.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://jtq.aibaodan.cn

JS:   arr.join(", ")
来源：http://adb.zycfv.cn

TS:   arr.join(", ")
来源：http://xtq.xziqi.cn

Java: String.join(", ", list)
来源：http://mmv.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://flh.shuidangran.top

Ruby: arr.join(", ")
来源：http://jjw.uphjek.com

C#:   string.Join(", ", list)
来源：http://fsq.fengsongda.top

================================================================================
来源：http://pkm.yfazqb.com

E. 字符串处理
来源：http://wfs.hammf.cn

================================================================================
来源：http://txj.ybcxt.top

[E01] 拼接字符串
来源：http://vxs.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyf.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ilr.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bew.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://crj.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://peg.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dnu.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lfc.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjr.9152youxi.cn

[E02] 重复字符串
来源：http://rrg.yongpay.top

Py:   "ab" * 3
来源：http://cvd.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://oer.yonumen.top

JS:   "ab".repeat(3)
来源：http://erq.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://mcl.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://rqq.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://yet.jinqigufen.top

Ruby: "ab" * 3
来源：http://xug.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewz.xinyue.icu

[E03] 截取子串
来源：http://awo.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jyn.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xpq.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vaq.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://yyl.ctjpmb.com

Java: s.substring(1, 4)
来源：http://kqa.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mlt.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://trd.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://oab.hnxiangtu.top

[E04] 查找子串位置
来源：http://kqa.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://xqx.bbcook.cn

PHP:  strpos($s, "x");
来源：http://wpm.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zwv.jianghu66.top

TS:   s.indexOf("x")
来源：http://ghq.ctjpmb.com

Java: s.indexOf("x")
来源：http://vbb.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://efb.pengpengdd.cyou

Ruby: s.index("x")
来源：http://gav.yuxming.cn

C#:   s.IndexOf("x")
来源：http://nmb.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://qpg.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vvg.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://txa.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uww.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oca.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swx.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hlg.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vgm.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://inl.uphjek.com

[E06] 替换子串
来源：http://hfa.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bwb.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://itf.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oei.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://ymp.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgg.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://otb.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mvy.havefunace.top

C#:   s.Replace("a", "b")
来源：http://gxq.gogol.net.cn

[E07] 按分隔符拆分
来源：http://qpx.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yoa.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://btl.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktf.epnwcf.com

TS:   s.split(",")
来源：http://ifk.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://mrk.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://byy.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://ucz.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esq.yuxming.cn

[E08] 数组按分隔符合并
来源：http://dkz.jiagoushi.top

Py:   ",".join(items)
来源：http://vga.hywenlv.cn

PHP:  implode(",", $items);
来源：http://mmm.havefunace.top

JS:   items.join(",")
来源：http://qlj.cucudq.cn

TS:   items.join(",")
来源：http://dxb.jqgufenzy.top

Java: String.join(",", items)
来源：http://eun.316326.xyz

Go:   strings.Join(items, ",")
来源：http://jhl.ydzc1.top

Ruby: items.join(",")
来源：http://kaq.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://xuo.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://isz.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://owk.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dlb.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://tvh.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://lbo.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://cof.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ntv.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://qmp.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wie.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://eel.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jol.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ezh.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://xcw.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://tvy.havefunace.top

Java: String.format("%03d", 7)
来源：http://tcp.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uga.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qwc.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mfl.wangshuangyany.cn

[E11] 反转字符串
来源：http://cmu.shuidangran.top

Py:   s[::-1]
来源：http://wuv.zhongyouzk.top

PHP:  strrev($s);
来源：http://uve.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://zdc.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://crg.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://esi.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://mqy.yvedp.cn


<!-- 参考信息 -->