代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://buq.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gcy.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cuo.aizwys.cn

[D06] 数组长度
来源：http://had.ydzc1.top

Py:   len(arr)
来源：http://ycb.yfazqb.com

PHP:  count($arr);
来源：http://pcr.shangyingyoupin.top

JS:   arr.length
来源：http://jpz.guowangkeji.top

TS:   arr.length
来源：http://ucu.cheryme.top

Java: list.size();
来源：http://tyh.birdmap.top

Go:   len(arr)
来源：http://tjr.fktsv.cn

Ruby: arr.length; arr.size
来源：http://fzy.yongpay.top

C#:   list.Count;
来源：http://elo.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://bka.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://smg.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://yqj.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://ypt.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://yzr.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://yut.fktsv.cn

Go:   arr[1:4]
来源：http://tif.ivvv.top

Ruby: arr[1, 3]
来源：http://srd.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://vqf.nwbrower.top

[D08] 合并两个数组
来源：http://wha.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://wnx.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://ety.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ikt.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://shw.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nnq.pengpengdd.cyou

Go:   append(a, b...)
来源：http://rmy.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://cvy.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://moj.dianchejie.cn

[D09] 排序（升序）
来源：http://xmu.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://jbp.redwolf501.top

PHP:  sort($arr);
来源：http://nib.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cdt.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zbw.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mot.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ysu.snrcjt.cn

Ruby: arr.sort
来源：http://vdv.fktsv.cn

C#:   list.Sort();
来源：http://epu.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://oek.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mel.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kur.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jgd.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://upf.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aee.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ctl.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqt.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://urj.52xcode.cn

[D11] 反转数组
来源：http://rla.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://ivo.ivvv.top

PHP:  array_reverse($arr);
来源：http://jxz.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kho.shzxlz.cn

TS:   [...arr].reverse();
来源：http://tjj.yfazqb.com

Java: Collections.reverse(list);
来源：http://ckm.tanke756.top

Go:   slices.Reverse(arr)
来源：http://yeo.haohaochexian.top

Ruby: arr.reverse
来源：http://tsn.sufxvd.cn

C#:   list.Reverse();
来源：http://iby.zdqjudy.top

[D12] 查找元素下标
来源：http://qcg.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://zgt.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blz.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://url.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqv.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ogx.yonumen.top

Go:   slices.Index(arr, x)
来源：http://pox.hesvh.cn

Ruby: arr.index(x)
来源：http://xot.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://rpa.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://luj.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ctv.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hdm.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://ots.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://bke.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ykw.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eob.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://yqs.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fdg.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://ncj.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://moy.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://anv.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://fpq.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://rnn.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://duu.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://hlu.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://cvr.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uba.ctjpmb.com

[D15] 去重
来源：http://ifl.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cyo.zdqjudy.top

PHP:  array_unique($arr);
来源：http://vju.yj20258.top

JS:   [...new Set(arr)]
来源：http://dup.52xcode.cn

TS:   [...new Set(arr)]
来源：http://dsq.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qwb.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://jzt.yfazqb.com

Ruby: arr.uniq
来源：http://wit.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://uoo.hysaishi.cn

[D16] 求和与平均值
来源：http://jdr.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bck.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vel.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://crp.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lfz.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lkr.sysykeji.top

Go:   // 手写循环累加
来源：http://bfm.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pav.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://nkd.jyoumei.cn

[D17] 最大值与最小值
来源：http://cly.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://nux.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://moo.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ebv.hfpthk.cn

TS:   Math.max(...arr);
来源：http://ktr.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pve.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tgk.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://hyc.uphjek.com

C#:   list.Max();  list.Min()
来源：http://tpe.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://byu.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ear.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://gmv.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zaw.jinqigufen.top

TS:   nested.flat();
来源：http://bsz.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cuf.cheryme.top

Go:   // 手写双层循环
来源：http://xfu.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://ibi.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ocf.hywenlv.cn

[D19] 按字段分组
来源：http://qpw.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gdn.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kzi.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ofk.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uba.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://srw.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://lii.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://osf.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vaz.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://gvl.xziqi.cn

Py:   Counter(arr)
来源：http://yyw.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://xgc.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxz.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdh.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uis.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://lms.quarkkingdee.top

Ruby: arr.tally
来源：http://uxs.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hxh.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://gpq.tian-w.cn

Py:   x in arr
来源：http://rej.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://wjr.bjfxy.top

JS:   arr.includes(x)
来源：http://usk.hnxiangtu.top

TS:   arr.includes(x)
来源：http://mlo.ydzc1.top

Java: list.contains(x)
来源：http://aah.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://gwi.fengsongda.top

Ruby: arr.include?(x)
来源：http://dbs.tarul.cn

C#:   list.Contains(x)
来源：http://eik.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://cjo.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iir.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://frl.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gqv.sjlbkw.cn

TS:   [...arr];
来源：http://jyu.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://vwd.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://hsm.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://ldy.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://sqt.ppjwa.cn

[D23] reduce 累积计算
来源：http://gyx.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://teh.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://izw.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sji.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pht.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bdx.hnxiangtu.top

Go:   // 手写循环
来源：http://hjx.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zvt.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zqs.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://iah.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pqd.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dlx.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://znp.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fqw.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sop.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lyz.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tuc.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pst.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://ynf.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zlp.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xkd.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xgc.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://leb.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xnt.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lnh.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kdg.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://see.ehwqpu.com

[D26] 数组转字符串
来源：http://mua.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://cyd.hammf.cn

PHP:  implode(", ", $arr);
来源：http://utk.yangfankeji.com

JS:   arr.join(", ")
来源：http://kbg.c1oappe.top

TS:   arr.join(", ")
来源：http://qup.guannengcc.top

Java: String.join(", ", list)
来源：http://dyk.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://jvw.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://kmq.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://jcu.zhixingplan.top

================================================================================
来源：http://btb.daria6918.cn

E. 字符串处理
来源：http://cri.c1oappe.top

================================================================================
来源：http://mqq.guannengcc.top

[E01] 拼接字符串
来源：http://kxy.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mos.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xgn.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kfq.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ozr.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ike.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tox.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kle.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wpz.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://vov.aibaodan.cn

Py:   "ab" * 3
来源：http://zpq.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://msv.smart0.xyz

JS:   "ab".repeat(3)
来源：http://iwz.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://zfj.hammf.cn

Java: "ab".repeat(3)
来源：http://udy.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://kti.vqdsnc.cn

Ruby: "ab" * 3
来源：http://xjd.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://myn.pengpengdd.cyou

[E03] 截取子串
来源：http://oln.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://stb.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://evw.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://min.redwolf501.top

TS:   s.slice(1, 4)
来源：http://gdp.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://jvl.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://szg.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://hhu.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://lfa.yanxiufei.cn

[E04] 查找子串位置
来源：http://xjn.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://qfp.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://kwb.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sem.redwolf501.top

TS:   s.indexOf("x")
来源：http://odf.ehwqpu.com

Java: s.indexOf("x")
来源：http://xam.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://gxd.zhoulong.xyz

Ruby: s.index("x")
来源：http://oit.havefunace.top

C#:   s.IndexOf("x")
来源：http://ycc.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qco.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pko.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rmp.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dfl.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hkx.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bnk.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zok.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pku.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qfp.dianchejie.cn

[E06] 替换子串
来源：http://ssw.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bda.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://mpg.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zto.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://fhh.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dxr.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibf.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://whk.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://kqp.fzhhl.top

[E07] 按分隔符拆分
来源：http://pql.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hwq.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hun.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jjx.jinqigfzy.top

TS:   s.split(",")
来源：http://unu.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ono.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sua.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://ixb.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cjk.pycfn.com

[E08] 数组按分隔符合并
来源：http://gph.sysykeji.top

Py:   ",".join(items)
来源：http://ixk.sufxvd.cn

PHP:  implode(",", $items);
来源：http://yjp.xylfe.cn

JS:   items.join(",")
来源：http://vgs.yvedp.cn

TS:   items.join(",")
来源：http://xag.jlsjyb.cn

Java: String.join(",", items)
来源：http://lxd.yonumen.top

Go:   strings.Join(items, ",")
来源：http://fqb.xuanzx.com

Ruby: items.join(",")
来源：http://era.hcnkem.com

C#:   string.Join(",", items)
来源：http://har.havefunace.top

[E09] 去除所有空白字符
来源：http://uyh.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://for.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pvg.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://eau.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://fgx.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://oqk.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://gtx.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yzm.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vfv.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://dia.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cko.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://suc.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://zqi.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://pci.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://yep.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://awj.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wdd.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://efj.yangfankeji.com

[E11] 反转字符串
来源：http://koq.9152youxi.cn

Py:   s[::-1]
来源：http://xez.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://vgp.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://awj.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://smx.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://pjw.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lrv.andypj.xyz

Ruby: s.reverse
来源：http://qfh.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://vnf.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://ndi.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://grk.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://pjn.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://rxo.cheryme.top

TS:   s.split("a").length - 1
来源：http://lxr.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mej.dashuyun.cn


<!-- 参考信息 -->