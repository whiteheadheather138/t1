代发 wailian999

[D07] 切片 / 取子数组
来源：http://ujr.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qic.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fpk.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://hdn.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://cjr.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://czz.cqqwz.cn

Go:   arr[1:4]
来源：http://dnz.cqqwz.cn

Ruby: arr[1, 3]
来源：http://tmj.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://cgk.mhx1999.top

[D08] 合并两个数组
来源：http://rzw.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://gsy.yonumen.top

PHP:  array_merge($a, $b);
来源：http://ors.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lzy.birdmap.top

TS:   [...a, ...b];
来源：http://ggz.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ume.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://rhy.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://myt.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://tws.cashguo.top

[D09] 排序（升序）
来源：http://iaz.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://doo.jinqigfzy.top

PHP:  sort($arr);
来源：http://lza.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zkb.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://aan.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kuh.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nyi.hnqzz.top

Ruby: arr.sort
来源：http://lnm.jinqigfzy.top

C#:   list.Sort();
来源：http://akl.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://psl.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dyb.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bhr.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://les.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hha.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvb.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vkr.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ogf.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fnr.hnqzz.top

[D11] 反转数组
来源：http://hvg.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ywi.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://ewh.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mxp.sxryk.cn

TS:   [...arr].reverse();
来源：http://nmj.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://axx.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://tjl.jinqigfzy.top

Ruby: arr.reverse
来源：http://rhv.dianchejie.cn

C#:   list.Reverse();
来源：http://vlb.xylfe.cn

[D12] 查找元素下标
来源：http://vsa.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://qxp.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uuc.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ciz.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sec.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mjh.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://wfi.jyoumei.cn

Ruby: arr.index(x)
来源：http://lzg.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://rlh.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://ktn.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://edz.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bje.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://gtu.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://mdn.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sit.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tje.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://dmf.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zir.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://hmv.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eai.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bvo.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://rdq.sweek.top

TS:   arr.map(x => x * 2)
来源：http://hyn.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fyp.xuanzx.com

Go:   // 手写循环
来源：http://kmu.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://lml.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gjv.sxryk.cn

[D15] 去重
来源：http://cga.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hup.cashguo.top

PHP:  array_unique($arr);
来源：http://uop.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://cof.hcnkem.com

TS:   [...new Set(arr)]
来源：http://mfc.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://exm.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yyi.dashuyun.cn

Ruby: arr.uniq
来源：http://xdp.sweek.top

C#:   list.Distinct().ToList()
来源：http://cyj.xylfe.cn

[D16] 求和与平均值
来源：http://ars.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bjw.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wdb.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zaz.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jau.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mrw.aibaodan.cn

Go:   // 手写循环累加
来源：http://qkh.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kil.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://pxt.kuanghao11.cn

[D17] 最大值与最小值
来源：http://bha.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://kyv.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://xxg.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mnv.ehwqpu.com

TS:   Math.max(...arr);
来源：http://ncn.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uux.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://poq.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://xwj.316326.xyz

C#:   list.Max();  list.Min()
来源：http://qfb.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://typ.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://obr.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://szq.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://weo.shzxlz.cn

TS:   nested.flat();
来源：http://pck.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gha.epnwcf.com

Go:   // 手写双层循环
来源：http://cno.xinyue.icu

Ruby: nested.flatten
来源：http://ntd.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://eyb.hammf.cn

[D19] 按字段分组
来源：http://kmi.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmw.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xuc.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://chf.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://ehc.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcb.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://fru.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rdj.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qol.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://iik.hesvh.cn

Py:   Counter(arr)
来源：http://fsx.hcnkem.com

PHP:  array_count_values($arr);
来源：http://drm.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oze.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jsq.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gdv.havefunace.top

Go:   // 手写 map[T]int
来源：http://gdp.nanxinkj.top

Ruby: arr.tally
来源：http://zjh.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jsg.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://pah.hnxiangtu.top

Py:   x in arr
来源：http://xit.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://ebk.havefunace.top

JS:   arr.includes(x)
来源：http://bnc.daxiang520.top

TS:   arr.includes(x)
来源：http://qnj.yfazqb.com

Java: list.contains(x)
来源：http://unr.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://ips.ivvv.top

Ruby: arr.include?(x)
来源：http://rxq.svipenyu.cn

C#:   list.Contains(x)
来源：http://vkm.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://spa.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xmh.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://avf.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfm.epnwcf.com

TS:   [...arr];
来源：http://wsc.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://jrv.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vin.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://tdm.tarul.cn

C#:   new List<int>(list);
来源：http://dbx.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://tdl.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gei.zdbjq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gbo.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxj.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjy.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://etn.pycfn.com

Go:   // 手写循环
来源：http://gxu.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jtc.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjn.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://xfw.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dah.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abp.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mzj.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mxh.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://haz.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tnz.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nui.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dod.ivvv.top

[D25] Set 集合去重与交并差
来源：http://nwg.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rmz.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pzn.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nna.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gbm.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qle.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uwj.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://coo.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ckb.jiagoushi.top

[D26] 数组转字符串
来源：http://rch.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://slc.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://aqc.kuanghao11.cn

JS:   arr.join(", ")
来源：http://nzn.zhongyouzk.top

TS:   arr.join(", ")
来源：http://psi.yueranfly.top

Java: String.join(", ", list)
来源：http://miv.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://yhd.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://tlf.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://ppc.gaohongyu789.top

================================================================================
来源：http://nzt.shuidangran.top

E. 字符串处理
来源：http://fzq.mhx1999.top

================================================================================
来源：http://gko.tanke756.top

[E01] 拼接字符串
来源：http://aov.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bxn.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qsq.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvg.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wef.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xfo.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wgx.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://trv.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mbh.nanxuanxn.top

[E02] 重复字符串
来源：http://vum.xylfe.cn

Py:   "ab" * 3
来源：http://zba.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://ken.cheryme.top

JS:   "ab".repeat(3)
来源：http://qwm.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://sdu.snrcjt.cn

Java: "ab".repeat(3)
来源：http://far.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://omh.mhx1999.top

Ruby: "ab" * 3
来源：http://wwf.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jkf.mhx1999.top

[E03] 截取子串
来源：http://nry.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cwc.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nef.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iif.meibo888.top

TS:   s.slice(1, 4)
来源：http://gmm.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://nul.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bdo.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://ccz.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://efj.9152youxi.cn

[E04] 查找子串位置
来源：http://qmq.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://gco.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://ney.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ehp.zycfv.cn

TS:   s.indexOf("x")
来源：http://lav.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://tgc.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://wpm.yuxming.cn

Ruby: s.index("x")
来源：http://skn.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://ews.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fee.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uyp.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hil.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcl.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iln.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybl.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hqi.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uxo.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ljt.aibaodan.cn

[E06] 替换子串
来源：http://dpp.0kj1m.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vqk.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://jna.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdu.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://try.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://okk.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://icw.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://azm.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://hdg.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://aud.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mfx.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ovn.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://moh.wangshuangyany.cn

TS:   s.split(",")
来源：http://yrb.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://nkb.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zya.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://ogy.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eks.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://gsg.wangshuangyany.cn

Py:   ",".join(items)
来源：http://loy.cheryme.top

PHP:  implode(",", $items);
来源：http://pek.vqdsnc.cn

JS:   items.join(",")
来源：http://blb.zdbjq.cn

TS:   items.join(",")
来源：http://qse.zhiwuduotai.top

Java: String.join(",", items)
来源：http://clp.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://vec.ehwqpu.com

Ruby: items.join(",")
来源：http://nla.svipenyu.cn

C#:   string.Join(",", items)
来源：http://bvi.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://eha.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tkg.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nek.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://kkk.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://yza.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://kzk.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tga.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://nvc.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://znx.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://ujh.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vxb.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nih.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://oze.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://gdt.bbcook.cn

Java: String.format("%03d", 7)
来源：http://jce.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fbb.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pmu.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://msn.fengsongda.top

[E11] 反转字符串
来源：http://xam.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://qmo.hfpthk.cn

PHP:  strrev($s);
来源：http://zzu.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://zdz.uphjek.com

TS:   [...s].reverse().join("")
来源：http://war.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hrh.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xxr.uphjek.com

Ruby: s.reverse
来源：http://rxp.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://wpy.daria6918.cn

[E12] 统计某字符出现次数
来源：http://obh.andypj.xyz

Py:   s.count("a")
来源：http://srb.birdmap.top

PHP:  substr_count($s, "a");
来源：http://qui.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://hlu.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://gms.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zjt.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://xuq.fktsv.cn

Ruby: s.count("a")
来源：http://feb.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://isd.smart0.xyz

[E13] 逐字符遍历
来源：http://clv.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://trp.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xln.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rga.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ywr.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tzw.gzhubu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://chg.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://yur.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ggz.hysaishi.cn


<!-- 参考信息 -->