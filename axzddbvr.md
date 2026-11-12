代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://nki.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://smu.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://bso.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bvv.iojbl.cn

PHP:  sort($arr);
来源：http://wrt.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tkg.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yjr.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fdg.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nks.hfpthk.cn

Ruby: arr.sort
来源：http://txo.c1oappe.top

C#:   list.Sort();
来源：http://zkt.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bas.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://box.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://snq.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://alv.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvy.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wrm.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wcv.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hvt.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qco.tian-w.cn

[D11] 反转数组
来源：http://umd.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://dhg.hesvh.cn

PHP:  array_reverse($arr);
来源：http://rzo.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfm.shuidangran.top

TS:   [...arr].reverse();
来源：http://brg.cheryme.top

Java: Collections.reverse(list);
来源：http://oyv.ivvv.top

Go:   slices.Reverse(arr)
来源：http://zkq.birdmap.top

Ruby: arr.reverse
来源：http://wwg.hnqzz.top

C#:   list.Reverse();
来源：http://jxt.feifeiyinyue.top

[D12] 查找元素下标
来源：http://yya.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://vkg.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://keh.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qve.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vke.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sly.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://oob.tarul.cn

Ruby: arr.index(x)
来源：http://hih.tian-w.cn

C#:   list.IndexOf(x);
来源：http://jay.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://gxj.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zcn.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxq.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://bpe.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://lyi.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uly.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qie.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://awm.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ymw.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://rmq.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://plo.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xfr.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://gwz.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://qfj.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oww.chenzaomai.com

Go:   // 手写循环
来源：http://nud.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://myi.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xpf.iojbl.cn

[D15] 去重
来源：http://hxn.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ncw.ppjwa.cn

PHP:  array_unique($arr);
来源：http://cfb.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://mdw.andypj.xyz

TS:   [...new Set(arr)]
来源：http://vyx.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sxs.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://lid.feifeiyinyue.top

Ruby: arr.uniq
来源：http://srm.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://liw.vqdsnc.cn

[D16] 求和与平均值
来源：http://ywm.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lop.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tfc.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tru.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xej.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qek.redwolf501.top

Go:   // 手写循环累加
来源：http://mng.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cln.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://kwr.jiagoushi.top

[D17] 最大值与最小值
来源：http://glt.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://ptk.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://thz.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://paj.ctjpmb.com

TS:   Math.max(...arr);
来源：http://jlz.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dma.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://csr.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://ooh.meibo888.top

C#:   list.Max();  list.Min()
来源：http://mlw.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://tgi.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vpl.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://wca.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kou.yuanzhike.top

TS:   nested.flat();
来源：http://myz.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kxw.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://ube.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://pgi.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgb.yonumen.top

[D19] 按字段分组
来源：http://zic.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bne.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nnj.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vdd.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hew.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kfp.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://rhv.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eic.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zmm.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://qfu.sufxvd.cn

Py:   Counter(arr)
来源：http://oqk.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://qfq.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxd.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rqd.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wqw.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://dml.havefunace.top

Ruby: arr.tally
来源：http://dig.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://koc.yj20258888.top

[D21] 判断是否包含某元素
来源：http://ymg.shanyushiyangtech.top

Py:   x in arr
来源：http://lmt.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://zpn.jiagoushi.top

JS:   arr.includes(x)
来源：http://bdu.yj20258888.top

TS:   arr.includes(x)
来源：http://ggg.yanxiufei.cn

Java: list.contains(x)
来源：http://bft.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://nmz.chenlongwang.top

Ruby: arr.include?(x)
来源：http://ell.zhongyouzk.top

C#:   list.Contains(x)
来源：http://ogv.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://dvs.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nsf.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://npx.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qup.chenjidiqi.icu

TS:   [...arr];
来源：http://seo.yj20258888.top

Java: new ArrayList<>(list);
来源：http://ugh.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://kfc.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://scu.c1oappe.top

C#:   new List<int>(list);
来源：http://tgo.kuanghao11.cn

[D23] reduce 累积计算
来源：http://xpi.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://etk.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lui.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfr.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://spa.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fty.sufxvd.cn

Go:   // 手写循环
来源：http://xyh.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bjx.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://epn.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://lyc.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wcx.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://try.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kvi.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vqj.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://edb.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://knn.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://szh.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oea.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://vnl.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zvs.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kvo.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kcv.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nns.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iee.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dqh.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bsi.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://suy.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://eih.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://edf.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://neg.xylfe.cn

JS:   arr.join(", ")
来源：http://mhi.zycfv.cn

TS:   arr.join(", ")
来源：http://cqp.hfpthk.cn

Java: String.join(", ", list)
来源：http://osr.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://lyf.mhx1999.top

Ruby: arr.join(", ")
来源：http://mpg.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://tqr.jqgufenzy.top

================================================================================
来源：http://jgr.xinyue.icu

E. 字符串处理
来源：http://dfm.xingfuxueyuan.xyz

================================================================================
来源：http://ljp.xuetiantiany.cn

[E01] 拼接字符串
来源：http://ioy.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ljr.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lkg.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fle.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlz.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://drv.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yij.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hst.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sgd.cqqwz.cn

[E02] 重复字符串
来源：http://hmk.bjfxy.top

Py:   "ab" * 3
来源：http://gpu.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://mcc.52xcode.cn

JS:   "ab".repeat(3)
来源：http://xhp.jianghu66.top

TS:   "ab".repeat(3)
来源：http://vvc.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://jox.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://xok.316326.xyz

Ruby: "ab" * 3
来源：http://hdb.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ukl.yuxming.cn

[E03] 截取子串
来源：http://ykv.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aaz.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mzt.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oeb.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://ngf.tianlin.xyz

Java: s.substring(1, 4)
来源：http://wkb.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hyl.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zjo.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://swb.cucudq.cn

[E04] 查找子串位置
来源：http://qsf.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://xiq.yonumen.top

PHP:  strpos($s, "x");
来源：http://ean.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dba.yongpay.top

TS:   s.indexOf("x")
来源：http://cxh.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://awo.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://usx.cqqwz.cn

Ruby: s.index("x")
来源：http://mti.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://hnd.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rgg.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nny.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://teg.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ylj.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ssr.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snv.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tfo.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://afk.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aum.jinqigufen.top

[E06] 替换子串
来源：http://lcl.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bze.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://pfs.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fmb.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://ipx.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xqy.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xen.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lks.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://vfe.sweek.top

[E07] 按分隔符拆分
来源：http://keh.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kad.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ppu.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ocm.jinqigfzy.top

TS:   s.split(",")
来源：http://ask.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rpj.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rbl.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://pct.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nmd.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://ufb.0kj1m.cn

Py:   ",".join(items)
来源：http://fuv.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://sfm.sufxvd.cn

JS:   items.join(",")
来源：http://pst.fehbvm.com

TS:   items.join(",")
来源：http://zxl.9152youxi.cn

Java: String.join(",", items)
来源：http://lph.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://qsd.hnqzz.top

Ruby: items.join(",")
来源：http://bmd.zdbjq.cn

C#:   string.Join(",", items)
来源：http://rdr.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://yst.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wqd.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wbm.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://iod.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://jiz.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://xtk.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://skm.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://utb.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gme.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://pak.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qjf.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsz.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://kpa.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://tfw.sweek.top

Java: String.format("%03d", 7)
来源：http://lpz.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ugl.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wvh.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rsf.wangdashe.top

[E11] 反转字符串
来源：http://sum.aibaodan.cn

Py:   s[::-1]
来源：http://fon.feifeiyinyue.top

PHP:  strrev($s);
来源：http://qxn.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://emg.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://rdv.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://djd.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lpj.ydzc1.top

Ruby: s.reverse
来源：http://iaq.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hwb.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://vja.fanxiaobao.xyz

Py:   s.count("a")
来源：http://keu.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://mdl.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://qde.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://iko.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fxq.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://iom.dashuyun.cn

Ruby: s.count("a")
来源：http://tpe.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://uus.vqdsnc.cn

[E13] 逐字符遍历
来源：http://jbi.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://qur.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oub.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pie.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://cxm.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iju.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jdq.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hnw.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yqo.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://ern.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvu.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://kno.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rtw.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://olu.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igl.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ody.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://foe.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsa.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://ivf.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lke.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://siu.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://omt.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jtq.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ece.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://udp.zdbjq.cn


<!-- 参考信息 -->