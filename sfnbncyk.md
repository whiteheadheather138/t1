代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wee.sxryk.cn

Ruby: arr.sort
来源：http://xfs.zhengqikj.top

C#:   list.Sort();
来源：http://dzy.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sxq.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mlu.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbr.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jef.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://trk.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ajj.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yzr.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hle.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nfd.bbcook.cn

[D11] 反转数组
来源：http://cxk.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://wkw.yj20258.top

PHP:  array_reverse($arr);
来源：http://exn.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xty.yangfankeji.com

TS:   [...arr].reverse();
来源：http://ujl.zycfv.cn

Java: Collections.reverse(list);
来源：http://ucg.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://xjx.yuxming.cn

Ruby: arr.reverse
来源：http://pys.jinqigufen.top

C#:   list.Reverse();
来源：http://mop.chenlongwang.top

[D12] 查找元素下标
来源：http://qgc.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://fco.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bto.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kjh.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqy.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://otg.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://nym.xylfe.cn

Ruby: arr.index(x)
来源：http://amn.52xcode.cn

C#:   list.IndexOf(x);
来源：http://mjk.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://fwb.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zvq.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jsl.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://orv.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://qeh.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lge.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yzg.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://aas.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xof.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://lhn.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fmm.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dyb.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://agx.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://ibz.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wml.zhoulong.xyz

Go:   // 手写循环
来源：http://qjg.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cpq.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://sfh.tanke756.top

[D15] 去重
来源：http://nvz.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yti.yvedp.cn

PHP:  array_unique($arr);
来源：http://bna.bbcook.cn

JS:   [...new Set(arr)]
来源：http://uvo.tanke756.top

TS:   [...new Set(arr)]
来源：http://mgk.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nyy.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://csc.xuetiantiany.cn

Ruby: arr.uniq
来源：http://ahp.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://gqw.sxryk.cn

[D16] 求和与平均值
来源：http://fvq.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvx.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rhm.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xdx.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcu.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qbx.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://hae.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lpt.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://wdy.aibaodan.cn

[D17] 最大值与最小值
来源：http://jvx.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://xab.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://dcr.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qxz.pycfn.com

TS:   Math.max(...arr);
来源：http://ioa.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://hpi.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kln.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://jno.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://yie.yonumen.top

[D18] 扁平化嵌套数组
来源：http://tkw.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ivk.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://ubb.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://urj.daria6918.cn

TS:   nested.flat();
来源：http://klc.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://etd.fehbvm.com

Go:   // 手写双层循环
来源：http://edx.havefunace.top

Ruby: nested.flatten
来源：http://pfn.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://htn.uphjek.com

[D19] 按字段分组
来源：http://lrt.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gan.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gko.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://khv.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mik.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://exs.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://tbv.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ayn.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://clg.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://nir.yueranfly.top

Py:   Counter(arr)
来源：http://sdf.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://uhu.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gal.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwq.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oxd.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://gxo.ppjwa.cn

Ruby: arr.tally
来源：http://wuo.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://grh.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://ukd.hesvh.cn

Py:   x in arr
来源：http://efk.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://udm.hcnkem.com

JS:   arr.includes(x)
来源：http://ztw.hcnkem.com

TS:   arr.includes(x)
来源：http://gra.ctjpmb.com

Java: list.contains(x)
来源：http://dwe.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://ltc.sxryk.cn

Ruby: arr.include?(x)
来源：http://ieg.316326.xyz

C#:   list.Contains(x)
来源：http://iqn.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://htw.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zab.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sqn.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfp.vqdsnc.cn

TS:   [...arr];
来源：http://fqn.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://ghg.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qvc.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://zxx.aizwys.cn

C#:   new List<int>(list);
来源：http://wqu.nwbrower.top

[D23] reduce 累积计算
来源：http://jhg.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wbf.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zbr.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wvm.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyo.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oqf.hammf.cn

Go:   // 手写循环
来源：http://pnr.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xho.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kou.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://ahn.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mth.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://klk.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://efk.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qsk.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iys.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://stk.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cqk.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://egj.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://xoz.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pia.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://irh.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rhi.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://akb.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qne.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxh.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://heb.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nsb.hnxiangtu.top

[D26] 数组转字符串
来源：http://gzl.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://qwm.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://daz.bjfxy.top

JS:   arr.join(", ")
来源：http://wei.jqgfzy.top

TS:   arr.join(", ")
来源：http://zmj.yuxming.cn

Java: String.join(", ", list)
来源：http://tcp.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://bxu.hnqzz.top

Ruby: arr.join(", ")
来源：http://pqp.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://mba.kuanghao11.cn

================================================================================
来源：http://fli.chenjidiqi.icu

E. 字符串处理
来源：http://fmm.hammf.cn

================================================================================
来源：http://odh.sweek.top

[E01] 拼接字符串
来源：http://vss.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hli.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kji.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tcy.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qyi.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aht.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bzq.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://buw.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://awl.nwbrower.top

[E02] 重复字符串
来源：http://ncb.nanxuanxn.top

Py:   "ab" * 3
来源：http://glm.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://cny.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://qhx.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://ffc.9152youxi.cn

Java: "ab".repeat(3)
来源：http://bca.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://jro.jinqigfzy.top

Ruby: "ab" * 3
来源：http://edr.guannengcc.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xkh.ivvv.top

[E03] 截取子串
来源：http://ors.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rlw.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aiv.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ckz.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://wcp.epnwcf.com

Java: s.substring(1, 4)
来源：http://hmt.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tde.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://cdx.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://dxr.jinqigfzy.top

[E04] 查找子串位置
来源：http://wml.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://cik.yj20258.top

PHP:  strpos($s, "x");
来源：http://lgk.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gzo.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://emn.hnqzz.top

Java: s.indexOf("x")
来源：http://lsv.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://dtm.kuanghao11.cn

Ruby: s.index("x")
来源：http://bul.xinyue.icu

C#:   s.IndexOf("x")
来源：http://oku.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://caf.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zbo.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jqd.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zpb.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://laj.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://isx.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://djg.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cdn.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rvy.sjlbkw.cn

[E06] 替换子串
来源：http://csa.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ell.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://ebh.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrh.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://wns.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qoi.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tit.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mal.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://jeh.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://rjd.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hmn.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jij.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ybc.birdmap.top

TS:   s.split(",")
来源：http://han.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://vxw.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mdx.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://gel.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pid.yj20258.top

[E08] 数组按分隔符合并
来源：http://guf.yongpay.top

Py:   ",".join(items)
来源：http://tij.yangfankeji.com

PHP:  implode(",", $items);
来源：http://ooj.jinqigufen.top

JS:   items.join(",")
来源：http://any.yongpay.top

TS:   items.join(",")
来源：http://adr.yj20258888.top

Java: String.join(",", items)
来源：http://gvj.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://mel.yj202588.top

Ruby: items.join(",")
来源：http://gnm.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://ggu.dashuyun.cn

[E09] 去除所有空白字符
来源：http://vji.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jcq.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ntq.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://uyl.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://iwk.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://abl.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dbb.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://ckc.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tcc.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://mso.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mmc.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ovf.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://bkx.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://bwf.yonumen.top

Java: String.format("%03d", 7)
来源：http://jlw.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://edj.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dlh.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nkv.wangdashe.top

[E11] 反转字符串
来源：http://skb.gzhubu.top

Py:   s[::-1]
来源：http://gvc.zdqjudy.top

PHP:  strrev($s);
来源：http://myn.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://soo.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://rni.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lel.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tlh.cdnleiting.top

Ruby: s.reverse
来源：http://pbw.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://tsr.c1oappe.top

[E12] 统计某字符出现次数
来源：http://zyn.snrcjt.cn

Py:   s.count("a")
来源：http://hsd.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://npj.yj20258888.top

JS:   s.split("a").length - 1
来源：http://gvz.hnqzz.top

TS:   s.split("a").length - 1
来源：http://otb.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rpb.316326.xyz

Go:   strings.Count(s, "a")
来源：http://khk.guowangkeji.top

Ruby: s.count("a")
来源：http://bpf.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://uyp.daria6918.cn

[E13] 逐字符遍历
来源：http://aap.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://pvm.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tto.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jql.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rga.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zgw.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ldb.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cci.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ggf.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://tjc.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mgk.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vrt.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vci.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vqw.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ahd.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mmt.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fgu.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nxh.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://ytg.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gaa.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kkm.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://stt.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ewv.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qaa.havefunace.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://guq.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zjv.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lzu.yanxiufei.cn

[E16] 数字千分位
来源：http://iop.sweek.top

Py:   f"{1234567:,}"
来源：http://fni.jiagoushi.top

PHP:  number_format(1234567);
来源：http://inb.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mzq.aibaodan.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rnd.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pxr.hfpthk.cn


<!-- 参考信息 -->