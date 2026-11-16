代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://jxh.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://elw.ctjpmb.com

[D09] 排序（升序）
来源：http://qhd.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://uox.aibaodan.cn

PHP:  sort($arr);
来源：http://krg.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cvh.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ymr.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xdn.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://giy.sweek.top

Ruby: arr.sort
来源：http://rmk.sufxvd.cn

C#:   list.Sort();
来源：http://asx.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tfg.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://haz.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyz.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oib.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://war.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xgx.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://onl.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edy.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ieb.daria6918.cn

[D11] 反转数组
来源：http://bcw.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://edt.ybcxt.top

PHP:  array_reverse($arr);
来源：http://sct.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://map.yongpay.top

TS:   [...arr].reverse();
来源：http://yon.dashuyun.cn

Java: Collections.reverse(list);
来源：http://mol.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://gzp.ehwqpu.com

Ruby: arr.reverse
来源：http://hmo.cucudq.cn

C#:   list.Reverse();
来源：http://xij.sjlbkw.cn

[D12] 查找元素下标
来源：http://gjy.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://eje.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wxh.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://puy.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hpr.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://htw.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://aeh.fengsongda.top

Ruby: arr.index(x)
来源：http://rdg.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://zlk.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://jrz.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjw.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vwr.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://njn.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://dyr.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jwc.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ggo.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ozg.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wvp.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://zdz.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://flx.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lkd.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://lzl.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://myj.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://hbq.fehbvm.com

Go:   // 手写循环
来源：http://thr.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://zul.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oyy.birdmap.top

[D15] 去重
来源：http://dfo.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tme.snrcjt.cn

PHP:  array_unique($arr);
来源：http://cvn.pycfn.com

JS:   [...new Set(arr)]
来源：http://ccv.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://ldd.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nyz.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cmh.uphjek.com

Ruby: arr.uniq
来源：http://jqq.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://lds.chenjidiqi.icu

[D16] 求和与平均值
来源：http://cbn.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wkt.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ecc.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxj.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejz.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvu.wangdashe.top

Go:   // 手写循环累加
来源：http://ntg.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qxy.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://qgs.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://uyy.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://gxf.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://ril.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oph.ivvv.top

TS:   Math.max(...arr);
来源：http://tfr.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lit.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xyr.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://mvi.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://rhm.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://uay.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vgb.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://oox.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wrf.xuetiantiany.cn

TS:   nested.flat();
来源：http://fwa.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sjc.havefunace.top

Go:   // 手写双层循环
来源：http://qlo.zhiwuduotai.top

Ruby: nested.flatten
来源：http://jdr.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://msq.fktsv.cn

[D19] 按字段分组
来源：http://jxi.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bir.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lje.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ryn.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://kok.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://omd.ivvv.top

Go:   // 手写 map[string][]T
来源：http://rjd.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wll.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://trc.sweek.top

[D20] 统计每个元素出现次数
来源：http://zqb.quarkkingdee.top

Py:   Counter(arr)
来源：http://wne.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://tjo.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dbz.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twm.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sgv.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://ahk.cdnleiting.top

Ruby: arr.tally
来源：http://wdp.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sfa.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://ufe.9152youxi.cn

Py:   x in arr
来源：http://dmr.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://olo.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://zos.svipenyu.cn

TS:   arr.includes(x)
来源：http://ehx.gogol.net.cn

Java: list.contains(x)
来源：http://nwh.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://vsp.bbcook.cn

Ruby: arr.include?(x)
来源：http://fii.aizwys.cn

C#:   list.Contains(x)
来源：http://gie.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://fvv.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpa.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jfx.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wjp.jyoumei.cn

TS:   [...arr];
来源：http://zgh.pycfn.com

Java: new ArrayList<>(list);
来源：http://mkr.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://dgs.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://gtz.ydzc1.top

C#:   new List<int>(list);
来源：http://vra.tian-w.cn

[D23] reduce 累积计算
来源：http://kdo.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vfp.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tvu.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vcc.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfe.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://jeh.yuxming.cn

Go:   // 手写循环
来源：http://jye.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uex.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pzl.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://akz.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyl.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://orv.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yae.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eum.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yxp.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xec.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uao.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zep.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://nco.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zma.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://woc.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xce.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oli.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xlx.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sbg.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vva.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dyp.guowangkeji.top

[D26] 数组转字符串
来源：http://jss.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://jjg.pycfn.com

PHP:  implode(", ", $arr);
来源：http://rjt.daria6918.cn

JS:   arr.join(", ")
来源：http://fbx.tianlin.xyz

TS:   arr.join(", ")
来源：http://zyo.gogol.net.cn

Java: String.join(", ", list)
来源：http://hra.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://etd.haohaochexian.top

Ruby: arr.join(", ")
来源：http://mog.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://azu.hcnkem.com

================================================================================
来源：http://ncp.ppjwa.cn

E. 字符串处理
来源：http://ges.hywenlv.cn

================================================================================
来源：http://gdt.fengsongda.top

[E01] 拼接字符串
来源：http://obd.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dlu.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tuc.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dzo.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://myc.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://utw.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://czj.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vat.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wxg.zdqjudy.top

[E02] 重复字符串
来源：http://gmg.yonumen.top

Py:   "ab" * 3
来源：http://luk.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://hol.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://wzp.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://gjx.bbcook.cn

Java: "ab".repeat(3)
来源：http://zgu.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://mul.xuanzx.com

Ruby: "ab" * 3
来源：http://efx.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://foq.aizwys.cn

[E03] 截取子串
来源：http://xta.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bia.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://okh.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mol.fzhhl.top

TS:   s.slice(1, 4)
来源：http://kua.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://ohv.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dsm.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://vok.ivvv.top

C#:   s.Substring(1, 3)
来源：http://ylu.zhengqikj.top

[E04] 查找子串位置
来源：http://kqm.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://xbi.wangdashe.top

PHP:  strpos($s, "x");
来源：http://hse.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zhz.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://vrx.yueranfly.top

Java: s.indexOf("x")
来源：http://epl.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://cgq.chenjidiqi.icu

Ruby: s.index("x")
来源：http://uch.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://qqt.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jcl.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ddo.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jdk.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ixj.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pju.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpy.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nab.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvo.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wyd.andypj.xyz

[E06] 替换子串
来源：http://kfr.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qna.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://zdw.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjr.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://lvp.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ogx.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vtx.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ydd.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://tvu.ydzc1.top

[E07] 按分隔符拆分
来源：http://fac.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aga.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uvg.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://zhf.bjfxy.top

TS:   s.split(",")
来源：http://rbi.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://olq.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pgv.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://tyo.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://odf.guannengcc.top

[E08] 数组按分隔符合并
来源：http://rro.fktsv.cn

Py:   ",".join(items)
来源：http://smy.chenzaomai.com

PHP:  implode(",", $items);
来源：http://ytj.dashuyun.cn

JS:   items.join(",")
来源：http://hlf.bjfxy.top

TS:   items.join(",")
来源：http://tmc.gzhubu.top

Java: String.join(",", items)
来源：http://bte.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://ani.316326.xyz

Ruby: items.join(",")
来源：http://kic.andypj.xyz

C#:   string.Join(",", items)
来源：http://ybs.gogol.net.cn

[E09] 去除所有空白字符
来源：http://nph.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wng.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ryx.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://yez.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://muo.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://gjl.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxs.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gbi.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fky.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://gzz.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mjv.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vbs.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://fil.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://gtf.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://gvi.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vfp.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wpz.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dor.sweek.top

[E11] 反转字符串
来源：http://imv.ydzc1.top

Py:   s[::-1]
来源：http://izv.jinqigufen.top

PHP:  strrev($s);
来源：http://bam.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://qxx.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://pnn.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yyb.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ekb.nwbrower.top

Ruby: s.reverse
来源：http://iim.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://plg.c1oappe.top

[E12] 统计某字符出现次数
来源：http://pdr.zycfv.cn

Py:   s.count("a")
来源：http://cck.yonumen.top

PHP:  substr_count($s, "a");
来源：http://wcy.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://ign.xylfe.cn

TS:   s.split("a").length - 1
来源：http://auj.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xtr.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://orv.shangyingyoupin.top

Ruby: s.count("a")
来源：http://ihs.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://usd.jqgfzy.top

[E13] 逐字符遍历
来源：http://nrj.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://qhd.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://emy.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxw.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bmb.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hzg.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kvm.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uqs.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://syb.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://uba.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yny.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://roe.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zxn.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yjb.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vle.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sec.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uyi.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sbc.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://oiw.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://lvb.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rwf.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eyw.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uua.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://num.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://llx.yj20258888.top


<!-- 参考信息 -->