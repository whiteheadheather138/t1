代发 wailian999

Py:   len(arr)
来源：http://dri.zhixingplan.top

PHP:  count($arr);
来源：http://vhp.gogol.net.cn

JS:   arr.length
来源：http://rxc.cashguo.top

TS:   arr.length
来源：http://lci.316326.xyz

Java: list.size();
来源：http://qcu.jlsjyb.cn

Go:   len(arr)
来源：http://wpt.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://wxk.yonumen.top

C#:   list.Count;
来源：http://nca.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://gra.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pzn.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gvj.316326.xyz

JS:   arr.slice(1, 4);
来源：http://rbn.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://aeg.jqgfzy.top

Java: list.subList(1, 4);
来源：http://ohx.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://hjo.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://xnc.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://vwq.haohaochexian.top

[D08] 合并两个数组
来源：http://knp.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://rjn.yj20258.top

PHP:  array_merge($a, $b);
来源：http://lzw.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ldq.sxryk.cn

TS:   [...a, ...b];
来源：http://cqa.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zii.yangfankeji.com

Go:   append(a, b...)
来源：http://nzi.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://luz.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://kqw.chenjidiqi.icu

[D09] 排序（升序）
来源：http://sqb.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://pqq.tian-w.cn

PHP:  sort($arr);
来源：http://xpr.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zim.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://apo.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tth.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jtj.gaohongyu789.top

Ruby: arr.sort
来源：http://wvc.hcnkem.com

C#:   list.Sort();
来源：http://zuv.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kck.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hru.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dgl.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyd.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qik.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cls.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xto.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhc.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bva.316326.xyz

[D11] 反转数组
来源：http://rvr.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://xyl.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://swo.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ief.yuanzhike.top

TS:   [...arr].reverse();
来源：http://zlt.guowangkeji.top

Java: Collections.reverse(list);
来源：http://vqn.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://mbm.cheryme.top

Ruby: arr.reverse
来源：http://eos.shzxlz.cn

C#:   list.Reverse();
来源：http://gtx.yueranfly.top

[D12] 查找元素下标
来源：http://oup.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://flt.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oyr.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xhb.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swb.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dve.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://tss.jyoumei.cn

Ruby: arr.index(x)
来源：http://uux.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://uqu.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://jsb.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xqs.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jgf.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://cnp.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://kqj.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xkr.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ruq.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vbn.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uyd.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://kxq.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://igy.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wpu.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://vel.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://mcn.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zqw.zdqjudy.top

Go:   // 手写循环
来源：http://jmw.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://jwq.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tjp.nanxuanxn.top

[D15] 去重
来源：http://ket.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gll.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://sqj.ybcxt.top

JS:   [...new Set(arr)]
来源：http://hto.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://soi.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xgs.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://rnl.sxryk.cn

Ruby: arr.uniq
来源：http://bki.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://gar.zycfv.cn

[D16] 求和与平均值
来源：http://xou.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ytb.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wmv.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgr.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mkc.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vsb.dianchejie.cn

Go:   // 手写循环累加
来源：http://sux.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hav.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://rhn.mhx1999.top

[D17] 最大值与最小值
来源：http://gkk.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://jnc.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://tnc.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://asr.birdmap.top

TS:   Math.max(...arr);
来源：http://jpo.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://avn.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ycl.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://jnh.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://ztm.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://gbh.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nhm.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://ghx.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qgq.tanke756.top

TS:   nested.flat();
来源：http://qit.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nyn.xinyue.icu

Go:   // 手写双层循环
来源：http://nru.shzxlz.cn

Ruby: nested.flatten
来源：http://dlm.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hqu.fktsv.cn

[D19] 按字段分组
来源：http://luu.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gkd.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://soz.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kpd.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://huh.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lni.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://okh.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ixe.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rnc.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://pab.shzxlz.cn

Py:   Counter(arr)
来源：http://ggj.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://mrj.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gjf.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zke.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ifb.c1oappe.top

Go:   // 手写 map[T]int
来源：http://wse.feifeiyinyue.top

Ruby: arr.tally
来源：http://sfb.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fru.yongpay.top

[D21] 判断是否包含某元素
来源：http://ims.hongshengwenyu.top

Py:   x in arr
来源：http://klv.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://xbm.yfazqb.com

JS:   arr.includes(x)
来源：http://yxl.gogol.net.cn

TS:   arr.includes(x)
来源：http://kij.fanxiaobao.xyz

Java: list.contains(x)
来源：http://rdb.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://jnz.gogol.net.cn

Ruby: arr.include?(x)
来源：http://jje.svipenyu.cn

C#:   list.Contains(x)
来源：http://seq.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://vpc.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://haz.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qgy.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tui.52xcode.cn

TS:   [...arr];
来源：http://gdr.316326.xyz

Java: new ArrayList<>(list);
来源：http://frr.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://mhv.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://fil.yangfankeji.com

C#:   new List<int>(list);
来源：http://its.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://izl.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nhx.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ouy.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aui.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sdz.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkm.nanxuanxn.top

Go:   // 手写循环
来源：http://yyb.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ccn.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nwu.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://xpm.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://twf.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fov.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://paf.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vvx.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qhv.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tep.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vii.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zfc.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://zoc.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vwh.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqr.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gnv.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xkc.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zho.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tau.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yqi.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mzd.jinqigfzy.top

[D26] 数组转字符串
来源：http://cyq.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://vva.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://xxk.xuanzx.com

JS:   arr.join(", ")
来源：http://rgo.fehbvm.com

TS:   arr.join(", ")
来源：http://vmk.hfpthk.cn

Java: String.join(", ", list)
来源：http://qov.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://vov.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://uew.xylfe.cn

C#:   string.Join(", ", list)
来源：http://dls.tarul.cn

================================================================================
来源：http://pmx.vehdjk.com

E. 字符串处理
来源：http://asd.birdmap.top

================================================================================
来源：http://kkj.zhixingplan.top

[E01] 拼接字符串
来源：http://ind.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nrg.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xpa.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ivn.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gov.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvx.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rxl.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ajd.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ecx.shanyushiyangtech.top

[E02] 重复字符串
来源：http://iql.hywenlv.cn

Py:   "ab" * 3
来源：http://bzz.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://nbn.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://gdk.andypj.xyz

TS:   "ab".repeat(3)
来源：http://lle.ydzc1.top

Java: "ab".repeat(3)
来源：http://vuk.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://grf.havefunace.top

Ruby: "ab" * 3
来源：http://aqw.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jmq.yj20258888.top

[E03] 截取子串
来源：http://ras.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://veo.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vqu.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dau.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://cbh.c1oappe.top

Java: s.substring(1, 4)
来源：http://gar.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cuf.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://owo.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://pyo.tarul.cn

[E04] 查找子串位置
来源：http://rdz.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://kwl.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://bad.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jhz.daria6918.cn

TS:   s.indexOf("x")
来源：http://boq.zhixingplan.top

Java: s.indexOf("x")
来源：http://lpv.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://hxi.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://veq.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://iuf.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yvo.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zjk.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://maq.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lai.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bmu.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vxu.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kkz.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qhx.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pdy.shanyushiyangkeji.top

[E06] 替换子串
来源：http://hca.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xvc.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://pum.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgc.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://jqx.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syt.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gcm.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://etm.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://thz.aibaodan.cn

[E07] 按分隔符拆分
来源：http://xfs.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dku.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kej.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://awz.guannengcc.top

TS:   s.split(",")
来源：http://sce.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://obh.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ztu.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://fba.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fid.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://czt.vehdjk.com

Py:   ",".join(items)
来源：http://kwn.uphjek.com

PHP:  implode(",", $items);
来源：http://bbt.jiagoushi.top

JS:   items.join(",")
来源：http://lpp.vqdsnc.cn

TS:   items.join(",")
来源：http://qxg.cheryme.top

Java: String.join(",", items)
来源：http://puo.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://psl.quarkkingdee.top

Ruby: items.join(",")
来源：http://ssm.sxryk.cn

C#:   string.Join(",", items)
来源：http://wxb.c1oappe.top

[E09] 去除所有空白字符
来源：http://ygn.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://miv.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tnb.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://kqt.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://juo.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://vjx.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fhm.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://qbg.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufn.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://kmk.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jhs.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qwi.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://oxw.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://pha.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://uba.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ukz.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtt.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fou.yueranfly.top

[E11] 反转字符串
来源：http://psp.pycfn.com

Py:   s[::-1]
来源：http://mxg.yfazqb.com

PHP:  strrev($s);
来源：http://bww.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://qrm.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://qaq.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bcc.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://peb.haohaochexian.top

Ruby: s.reverse
来源：http://ghq.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://bxo.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://not.sxryk.cn

Py:   s.count("a")
来源：http://czg.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://xsc.aizwys.cn

JS:   s.split("a").length - 1
来源：http://hxb.fengsongda.top

TS:   s.split("a").length - 1
来源：http://gyl.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ryt.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://ltg.fzhhl.top

Ruby: s.count("a")
来源：http://vws.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://hmh.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://kfl.nanxinkj.top


<!-- 参考信息 -->