代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://npg.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vly.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://fkm.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://vkn.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zkm.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nrh.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hyr.tianlin.xyz

[D06] 数组长度
来源：http://mrf.snrcjt.cn

Py:   len(arr)
来源：http://kmi.jqgufenzy.top

PHP:  count($arr);
来源：http://oxb.yongpay.top

JS:   arr.length
来源：http://mvw.zhiwuduotai.top

TS:   arr.length
来源：http://sub.redwolf501.top

Java: list.size();
来源：http://zfz.ehwqpu.com

Go:   len(arr)
来源：http://mpt.xylfe.cn

Ruby: arr.length; arr.size
来源：http://ulw.daxiang520.top

C#:   list.Count;
来源：http://pib.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://bbj.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nul.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gco.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://qhs.tarul.cn

TS:   arr.slice(1, 4);
来源：http://kqk.jinqigufen.top

Java: list.subList(1, 4);
来源：http://gpd.cqqwz.cn

Go:   arr[1:4]
来源：http://dno.gzhubu.top

Ruby: arr[1, 3]
来源：http://dgp.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://hys.ivvv.top

[D08] 合并两个数组
来源：http://rcq.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://xyf.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://qqk.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nck.yueranfly.top

TS:   [...a, ...b];
来源：http://dsk.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zos.cucudq.cn

Go:   append(a, b...)
来源：http://vzk.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://tta.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://ltc.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://tog.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://fci.smart0.xyz

PHP:  sort($arr);
来源：http://peq.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sfg.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lak.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sio.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sfp.nwbrower.top

Ruby: arr.sort
来源：http://swu.sjlbkw.cn

C#:   list.Sort();
来源：http://otk.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hvh.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ykf.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czd.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbl.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vvp.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cma.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uiy.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jzi.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xlk.fktsv.cn

[D11] 反转数组
来源：http://blt.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ilf.wangdashe.top

PHP:  array_reverse($arr);
来源：http://akh.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lxu.haohaochexian.top

TS:   [...arr].reverse();
来源：http://vnl.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://llt.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://phx.yonumen.top

Ruby: arr.reverse
来源：http://hos.52xcode.cn

C#:   list.Reverse();
来源：http://zeh.316326.xyz

[D12] 查找元素下标
来源：http://ffy.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://tlw.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vba.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ena.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lql.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mnk.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://nbq.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://iyk.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://han.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://mor.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asp.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ksv.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://sdw.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://vch.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zge.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zpa.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ppd.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gxv.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://leq.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yir.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fky.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://zop.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://hrr.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eos.fengsongda.top

Go:   // 手写循环
来源：http://lsp.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://wdt.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://trh.52xcode.cn

[D15] 去重
来源：http://rbv.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uxt.nanxinkj.top

PHP:  array_unique($arr);
来源：http://nnm.ydzc1.top

JS:   [...new Set(arr)]
来源：http://pbn.yongpay.top

TS:   [...new Set(arr)]
来源：http://dwv.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpi.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pvk.316326.xyz

Ruby: arr.uniq
来源：http://mwz.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://ydx.ivvv.top

[D16] 求和与平均值
来源：http://tyk.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cro.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cno.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdr.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jba.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uhh.zdbjq.cn

Go:   // 手写循环累加
来源：http://wpj.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dwq.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://ylj.sweek.top

[D17] 最大值与最小值
来源：http://qwv.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://csh.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://ulr.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nwh.yonumen.top

TS:   Math.max(...arr);
来源：http://aim.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tfh.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ydt.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://gxy.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://zmb.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://ztk.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mlu.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://fot.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bsz.uphjek.com

TS:   nested.flat();
来源：http://eae.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wyv.tarul.cn

Go:   // 手写双层循环
来源：http://rvs.xuetiantiany.cn

Ruby: nested.flatten
来源：http://tit.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ugq.52xcode.cn

[D19] 按字段分组
来源：http://hif.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qeu.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qco.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iuf.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dkf.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sfm.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://xme.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fus.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yys.uphjek.com

[D20] 统计每个元素出现次数
来源：http://mat.hongshengwenyu.top

Py:   Counter(arr)
来源：http://wjj.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://wpo.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbh.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vfv.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lxl.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://tzg.aizwys.cn

Ruby: arr.tally
来源：http://jjq.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gvh.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://joi.havefunace.top

Py:   x in arr
来源：http://pfo.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://dpm.fehbvm.com

JS:   arr.includes(x)
来源：http://ctl.dianchejie.cn

TS:   arr.includes(x)
来源：http://unt.jqgufenzy.top

Java: list.contains(x)
来源：http://ocu.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://pdd.bjfxy.top

Ruby: arr.include?(x)
来源：http://ynt.ppjwa.cn

C#:   list.Contains(x)
来源：http://wzt.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://ocg.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zcf.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://npc.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tdf.hfpthk.cn

TS:   [...arr];
来源：http://xmk.ybcxt.top

Java: new ArrayList<>(list);
来源：http://fkx.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://afc.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://ujd.tarul.cn

C#:   new List<int>(list);
来源：http://wro.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://dcq.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpm.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ryr.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njk.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iht.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://zoq.chenjidiqi.icu

Go:   // 手写循环
来源：http://utt.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xvt.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zrl.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://kdv.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zyi.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pmd.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rqu.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://srd.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://olv.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vlz.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zop.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ryh.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://uvt.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tvy.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nfe.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://agh.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://elw.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oso.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jmj.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gve.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wcg.hnqzz.top

[D26] 数组转字符串
来源：http://yue.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://ngu.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://zjd.kuanghao11.cn

JS:   arr.join(", ")
来源：http://sde.yj20258.top

TS:   arr.join(", ")
来源：http://fux.sxryk.cn

Java: String.join(", ", list)
来源：http://wsh.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://vtx.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://uxg.xylfe.cn

C#:   string.Join(", ", list)
来源：http://aon.zhiwuduotai.top

================================================================================
来源：http://cid.c1oappe.top

E. 字符串处理
来源：http://pcw.gotoacloud.top

================================================================================
来源：http://uvq.gotoacloud.top

[E01] 拼接字符串
来源：http://jai.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dvs.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://btw.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dja.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqt.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sdu.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lrl.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://evg.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ywi.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://zjw.xziqi.cn

Py:   "ab" * 3
来源：http://vgw.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://uzt.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://bew.fktsv.cn

TS:   "ab".repeat(3)
来源：http://jjb.xinyue.icu

Java: "ab".repeat(3)
来源：http://fzs.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://pob.redwolf501.top

Ruby: "ab" * 3
来源：http://txd.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dtz.xinyue.icu

[E03] 截取子串
来源：http://anz.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iqp.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fza.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://naw.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://ryw.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://wps.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lif.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://eky.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://rws.svipenyu.cn

[E04] 查找子串位置
来源：http://uqd.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://ifr.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://cvc.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ztg.yj20258.top

TS:   s.indexOf("x")
来源：http://siv.xinyue.icu

Java: s.indexOf("x")
来源：http://peh.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://rcf.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://jfg.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://ofz.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://drq.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://opc.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zde.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hke.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wxh.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjo.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xig.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mzd.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://abk.hywenlv.cn

[E06] 替换子串
来源：http://cqo.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wev.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://hab.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktm.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://bvf.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wzb.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jxc.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://obc.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://bzb.0kj1m.cn

[E07] 按分隔符拆分
来源：http://rwu.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cky.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vfr.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://imd.chenjidiqi.icu

TS:   s.split(",")
来源：http://hyz.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://nhv.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ocb.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://osp.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vfw.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://ahu.fzhhl.top

Py:   ",".join(items)
来源：http://for.sysykeji.top

PHP:  implode(",", $items);
来源：http://cvp.jiagoushi.top

JS:   items.join(",")
来源：http://qxc.gogol.net.cn

TS:   items.join(",")
来源：http://akn.fehbvm.com

Java: String.join(",", items)
来源：http://hks.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://dgx.cdnleiting.top

Ruby: items.join(",")
来源：http://afu.guannengcc.top

C#:   string.Join(",", items)
来源：http://fmf.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://aot.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aab.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yjn.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://ykz.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://gjn.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://qes.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://okv.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dzk.jinqigfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aeo.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://zob.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yol.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tot.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://wjn.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://gla.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://nha.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zjt.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ejo.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mqv.tianlin.xyz

[E11] 反转字符串
来源：http://onu.haohaochexian.top

Py:   s[::-1]
来源：http://nzs.chenjidiqi.icu

PHP:  strrev($s);
来源：http://onz.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://oey.uphjek.com

TS:   [...s].reverse().join("")
来源：http://mui.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xdm.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hqx.sufxvd.cn

Ruby: s.reverse
来源：http://kxt.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ceh.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://poh.jqgufenzy.top

Py:   s.count("a")
来源：http://cdd.zycfv.cn


<!-- 参考信息 -->