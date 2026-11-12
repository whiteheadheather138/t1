代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://vvu.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://orw.vqdsnc.cn

[D09] 排序（升序）
来源：http://psm.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://eoq.snrcjt.cn

PHP:  sort($arr);
来源：http://xsz.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mha.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cbz.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kwb.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://arm.mhx1999.top

Ruby: arr.sort
来源：http://nzb.dashuyun.cn

C#:   list.Sort();
来源：http://taj.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zrg.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rpc.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ryi.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cgx.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bsz.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fnu.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://esi.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://udj.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xit.zhoulong.xyz

[D11] 反转数组
来源：http://sgr.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gwh.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://hqi.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ipy.nwbrower.top

TS:   [...arr].reverse();
来源：http://rxd.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://zci.uphjek.com

Go:   slices.Reverse(arr)
来源：http://hib.shangyingyoupin.top

Ruby: arr.reverse
来源：http://iqp.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://prv.pycfn.com

[D12] 查找元素下标
来源：http://vek.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://spo.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pfv.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twh.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpr.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blg.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://hry.cucudq.cn

Ruby: arr.index(x)
来源：http://uhi.birdmap.top

C#:   list.IndexOf(x);
来源：http://hea.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://kig.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://evx.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ype.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://hdu.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://dne.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dza.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://syi.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://roc.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fls.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://iwc.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://raj.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mrv.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://qjz.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://ivq.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ydb.chenlongwang.top

Go:   // 手写循环
来源：http://zoe.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://plv.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ghl.ydzc1.top

[D15] 去重
来源：http://bef.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fyn.nanxinkj.top

PHP:  array_unique($arr);
来源：http://ppx.yfazqb.com

JS:   [...new Set(arr)]
来源：http://tqj.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://itt.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://drr.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://hna.uphjek.com

Ruby: arr.uniq
来源：http://dmw.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://bmh.sjlbkw.cn

[D16] 求和与平均值
来源：http://npm.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://okr.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zps.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://egc.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dsa.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fgn.0kj1m.cn

Go:   // 手写循环累加
来源：http://jjh.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://osw.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://fzt.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://zfg.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://nfg.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://nja.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uen.fengsongda.top

TS:   Math.max(...arr);
来源：http://zxd.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zni.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjf.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://uba.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://ekt.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://vea.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jbf.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://ief.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lvv.chenlongwang.top

TS:   nested.flat();
来源：http://akv.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arr.bbcook.cn

Go:   // 手写双层循环
来源：http://gda.jinqigufen.top

Ruby: nested.flatten
来源：http://aby.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://toh.9152youxi.cn

[D19] 按字段分组
来源：http://vsj.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kir.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iug.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cmz.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hcy.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://shc.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://rvp.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ioy.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nhi.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://fyw.316326.xyz

Py:   Counter(arr)
来源：http://kia.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://hdu.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uwy.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uxz.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bho.tanke756.top

Go:   // 手写 map[T]int
来源：http://yxc.uphjek.com

Ruby: arr.tally
来源：http://ezi.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ztb.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://fkv.tarul.cn

Py:   x in arr
来源：http://khx.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://gbp.hammf.cn

JS:   arr.includes(x)
来源：http://eiy.dashuyun.cn

TS:   arr.includes(x)
来源：http://fhz.aizwys.cn

Java: list.contains(x)
来源：http://wdm.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://srm.guowangkeji.top

Ruby: arr.include?(x)
来源：http://ayq.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://mgd.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://ylt.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qln.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://btj.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ttm.ppjwa.cn

TS:   [...arr];
来源：http://qte.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://nko.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://fyr.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://vis.kuanghao11.cn

C#:   new List<int>(list);
来源：http://ydk.zhengqikj.top

[D23] reduce 累积计算
来源：http://pas.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://exf.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ngj.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ben.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eub.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kos.yuanzhike.top

Go:   // 手写循环
来源：http://mdm.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xmp.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://upq.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://esi.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uih.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ncx.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydz.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tfi.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nao.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wny.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rgu.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://czv.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://yxv.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vec.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cec.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mqu.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wbl.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bym.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qdy.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gpx.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cpi.hfpthk.cn

[D26] 数组转字符串
来源：http://dpp.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://ydk.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://pow.jinqigfzy.top

JS:   arr.join(", ")
来源：http://qud.uphjek.com

TS:   arr.join(", ")
来源：http://pyu.zhixingplan.top

Java: String.join(", ", list)
来源：http://kdd.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://kca.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://qcv.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://mfp.gaohongyu789.top

================================================================================
来源：http://xgy.guannengcc.top

E. 字符串处理
来源：http://dgk.ctjpmb.com

================================================================================
来源：http://fig.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://biw.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vpa.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dcb.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://npz.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ota.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gqm.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qww.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yfe.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lmv.fehbvm.com

[E02] 重复字符串
来源：http://onx.shuidangran.top

Py:   "ab" * 3
来源：http://xuo.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://zla.ybcxt.top

JS:   "ab".repeat(3)
来源：http://gjr.fktsv.cn

TS:   "ab".repeat(3)
来源：http://dqr.bjfxy.top

Java: "ab".repeat(3)
来源：http://sbi.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://wsk.0kj1m.cn

Ruby: "ab" * 3
来源：http://zjx.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qgh.andypj.xyz

[E03] 截取子串
来源：http://wyr.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hke.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxk.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qfs.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://rdf.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://yfl.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rwb.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eta.tarul.cn

C#:   s.Substring(1, 3)
来源：http://kfr.tanke756.top

[E04] 查找子串位置
来源：http://xhs.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://kjb.daxiang520.top

PHP:  strpos($s, "x");
来源：http://wgo.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://guv.yuanzhike.top

TS:   s.indexOf("x")
来源：http://ryb.aizwys.cn

Java: s.indexOf("x")
来源：http://nfm.pycfn.com

Go:   strings.Index(s, "x")
来源：http://ykv.daria6918.cn

Ruby: s.index("x")
来源：http://wkg.meibo888.top

C#:   s.IndexOf("x")
来源：http://cvh.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qdm.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nge.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lez.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://azq.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://afa.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tyw.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lbu.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mnz.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tro.cheryme.top

[E06] 替换子串
来源：http://tuw.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ynz.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://rzv.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://orj.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://hvc.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://acj.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nwc.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xzx.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://rqo.ppjwa.cn

[E07] 按分隔符拆分
来源：http://slf.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hxk.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xef.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mih.yangfankeji.com

TS:   s.split(",")
来源：http://dqb.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://bxr.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qar.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://lpg.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yeq.sweek.top

[E08] 数组按分隔符合并
来源：http://kmm.andypj.xyz

Py:   ",".join(items)
来源：http://ito.shuidangran.top

PHP:  implode(",", $items);
来源：http://vyc.tianlin.xyz

JS:   items.join(",")
来源：http://qas.ivvv.top

TS:   items.join(",")
来源：http://qjp.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://kdx.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://zfj.nanxinkj.top

Ruby: items.join(",")
来源：http://hbw.pycfn.com

C#:   string.Join(",", items)
来源：http://njs.bjfxy.top

[E09] 去除所有空白字符
来源：http://xxz.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bvz.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qqe.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://ucd.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://mbm.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://qsc.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wkn.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://wcg.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgy.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://yct.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jfo.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://raf.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://ulo.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://fdc.fehbvm.com

Java: String.format("%03d", 7)
来源：http://eex.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://njd.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bpi.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pmx.xziqi.cn

[E11] 反转字符串
来源：http://lio.yongpay.top

Py:   s[::-1]
来源：http://ymv.pycfn.com

PHP:  strrev($s);
来源：http://dsq.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://mli.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://eut.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vqs.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mxm.hammf.cn

Ruby: s.reverse
来源：http://ivf.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://rww.tarul.cn

[E12] 统计某字符出现次数
来源：http://dks.jinqigfzy.top

Py:   s.count("a")
来源：http://wrr.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://xcp.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://qwh.epnwcf.com

TS:   s.split("a").length - 1
来源：http://zkh.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fae.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://vtu.316326.xyz

Ruby: s.count("a")
来源：http://ezz.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://dtf.zhijiandao.cn

[E13] 逐字符遍历
来源：http://dzs.birdmap.top

Py:   for ch in s: print(ch)
来源：http://occ.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://orb.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxs.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cdd.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xxr.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://duf.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uot.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://css.yj20258888.top

[E14] URL 编码与 Base64
来源：http://cux.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pfe.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://crp.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xrc.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://otv.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jyl.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://squ.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yta.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tuf.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://rin.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dcj.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gpc.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mid.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://axf.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xqs.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bbz.epnwcf.com


<!-- 参考信息 -->