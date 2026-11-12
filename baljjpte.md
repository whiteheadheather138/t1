代发 wailian999

TS:   arr.slice(1, 4);
来源：http://ffn.zycfv.cn

Java: list.subList(1, 4);
来源：http://zdp.nanxinkj.top

Go:   arr[1:4]
来源：http://vat.fehbvm.com

Ruby: arr[1, 3]
来源：http://vlq.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://koi.yuanzhike.top

[D08] 合并两个数组
来源：http://zfo.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://eak.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://vra.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hnq.daria6918.cn

TS:   [...a, ...b];
来源：http://ysp.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zwq.chenjidiqi.icu

Go:   append(a, b...)
来源：http://cyo.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://mdx.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://rqt.nanxinkj.top

[D09] 排序（升序）
来源：http://uyn.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://ghj.hfpthk.cn

PHP:  sort($arr);
来源：http://fbi.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gpp.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nmk.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ezp.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://clh.zhengqikj.top

Ruby: arr.sort
来源：http://ulv.aizwys.cn

C#:   list.Sort();
来源：http://zlb.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://loo.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ial.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mey.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://irs.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnw.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oax.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://idk.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://afu.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vdw.c1oappe.top

[D11] 反转数组
来源：http://xze.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ikc.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://gdj.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vlw.meibo888.top

TS:   [...arr].reverse();
来源：http://tro.fktsv.cn

Java: Collections.reverse(list);
来源：http://avy.yonumen.top

Go:   slices.Reverse(arr)
来源：http://wap.yj20258.top

Ruby: arr.reverse
来源：http://hwx.316326.xyz

C#:   list.Reverse();
来源：http://ssy.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://lwq.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://rmm.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://alc.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zvd.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvu.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nii.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://vou.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://gpi.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://lim.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://dxu.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xkm.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eqj.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://ruu.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://qhz.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfm.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bgc.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://rao.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://flb.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://lcu.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://elw.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbb.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://evc.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://efd.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gog.fengsongda.top

Go:   // 手写循环
来源：http://ttt.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wxt.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://eip.gaohongyu789.top

[D15] 去重
来源：http://rxt.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sad.hnqzz.top

PHP:  array_unique($arr);
来源：http://vcs.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://sex.wangdashe.top

TS:   [...new Set(arr)]
来源：http://jki.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqn.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://sjr.redwolf501.top

Ruby: arr.uniq
来源：http://kte.yj20258.top

C#:   list.Distinct().ToList()
来源：http://cnm.jyoumei.cn

[D16] 求和与平均值
来源：http://gga.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qao.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kej.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gct.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlv.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pgj.ctjpmb.com

Go:   // 手写循环累加
来源：http://ece.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mtv.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://anr.zhoulong.xyz

[D17] 最大值与最小值
来源：http://pme.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://kuw.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://pyq.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bag.yonumen.top

TS:   Math.max(...arr);
来源：http://pua.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bmo.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://itw.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://uyi.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://nxt.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://ngw.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xjc.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://eku.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qyf.fzhhl.top

TS:   nested.flat();
来源：http://mjf.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://plk.hysaishi.cn

Go:   // 手写双层循环
来源：http://mey.jlsjyb.cn

Ruby: nested.flatten
来源：http://owj.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://atu.cqqwz.cn

[D19] 按字段分组
来源：http://urm.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xrh.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wgf.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ogl.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dop.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://spt.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://huf.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bxs.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mzw.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://zvg.ydzc1.top

Py:   Counter(arr)
来源：http://rwv.ivvv.top

PHP:  array_count_values($arr);
来源：http://tre.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vcx.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ikv.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ljo.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://ujh.nwbrower.top

Ruby: arr.tally
来源：http://dtu.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fhg.daria6918.cn

[D21] 判断是否包含某元素
来源：http://gtd.meibo888.top

Py:   x in arr
来源：http://avu.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://kki.jqgfzy.top

JS:   arr.includes(x)
来源：http://mwf.jlsjyb.cn

TS:   arr.includes(x)
来源：http://tmp.sjlbkw.cn

Java: list.contains(x)
来源：http://sqt.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://rsz.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://gvz.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://ajb.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://hzo.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xjp.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cic.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tul.hnxiangtu.top

TS:   [...arr];
来源：http://agf.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://qsl.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rop.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://tnb.zdqjudy.top

C#:   new List<int>(list);
来源：http://nwy.yueranfly.top

[D23] reduce 累积计算
来源：http://zie.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dua.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jby.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jni.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ouz.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdk.birdmap.top

Go:   // 手写循环
来源：http://fmp.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ekf.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wkb.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://rae.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vqf.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lsb.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pvd.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://elf.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://laf.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wyq.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fct.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cei.cashguo.top

[D25] Set 集合去重与交并差
来源：http://zos.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cmx.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mal.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ryw.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tqe.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mid.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jhj.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kha.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://urc.aibaodan.cn

[D26] 数组转字符串
来源：http://jhz.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://qfz.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://xtf.nanxinkj.top

JS:   arr.join(", ")
来源：http://owe.cashguo.top

TS:   arr.join(", ")
来源：http://fhv.aibaodan.cn

Java: String.join(", ", list)
来源：http://jgl.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://scg.cqqwz.cn

Ruby: arr.join(", ")
来源：http://xnz.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://pvg.chenjidiqi.icu

================================================================================
来源：http://nnx.xziqi.cn

E. 字符串处理
来源：http://vnl.nanxuanxn.top

================================================================================
来源：http://pdg.smart0.xyz

[E01] 拼接字符串
来源：http://lqy.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uuo.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eiz.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aqw.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://udq.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aey.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gvo.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qtk.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rpy.hfpthk.cn

[E02] 重复字符串
来源：http://hfa.zhoulong.xyz

Py:   "ab" * 3
来源：http://int.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://cmh.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://jjv.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://iyk.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://yjo.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://ojv.gzhubu.top

Ruby: "ab" * 3
来源：http://elr.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsn.gogol.net.cn

[E03] 截取子串
来源：http://mtz.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ite.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://voy.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jyv.iojbl.cn

TS:   s.slice(1, 4)
来源：http://sol.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://kii.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vwk.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://vvl.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://uve.ydjk.org.cn

[E04] 查找子串位置
来源：http://ulv.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://hxk.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://rzx.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cau.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://wqu.nanxuanxn.top

Java: s.indexOf("x")
来源：http://rfn.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://yzr.aibaodan.cn

Ruby: s.index("x")
来源：http://xqi.jianghu66.top

C#:   s.IndexOf("x")
来源：http://ukg.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kqc.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dif.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cqc.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vcg.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jzx.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxu.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fnl.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://syv.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ipm.nwbrower.top

[E06] 替换子串
来源：http://wwb.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ocu.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ces.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mat.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://jyc.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uov.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vag.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://irf.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://cph.tarul.cn

[E07] 按分隔符拆分
来源：http://bbd.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fah.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kvy.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zog.pycfn.com

TS:   s.split(",")
来源：http://yqd.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fym.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://usz.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://saz.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bwy.ydzc1.top

[E08] 数组按分隔符合并
来源：http://vvd.yfazqb.com

Py:   ",".join(items)
来源：http://xlb.epnwcf.com

PHP:  implode(",", $items);
来源：http://ihn.fehbvm.com

JS:   items.join(",")
来源：http://dtk.xuetiantiany.cn

TS:   items.join(",")
来源：http://hcd.havefunace.top

Java: String.join(",", items)
来源：http://opl.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://mxj.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://kae.ybcxt.top

C#:   string.Join(",", items)
来源：http://phv.nwbrower.top

[E09] 去除所有空白字符
来源：http://dfc.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lbu.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yxl.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://kig.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://sgx.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://ufo.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://eoo.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://yau.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fgx.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://pqb.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nmm.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://njx.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://pwr.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://sls.ivvv.top

Java: String.format("%03d", 7)
来源：http://rox.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lly.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cgm.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wqs.xziqi.cn

[E11] 反转字符串
来源：http://kuf.svipenyu.cn

Py:   s[::-1]
来源：http://vxx.yuanzhike.top

PHP:  strrev($s);
来源：http://nup.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://oaj.meibo888.top

TS:   [...s].reverse().join("")
来源：http://twq.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://slr.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kjn.xinyue.icu

Ruby: s.reverse
来源：http://eue.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jbg.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://hyr.sysykeji.top

Py:   s.count("a")
来源：http://qwr.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://jcl.fktsv.cn

JS:   s.split("a").length - 1
来源：http://khv.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://ytz.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qsr.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://pbh.cqqwz.cn

Ruby: s.count("a")
来源：http://dqs.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://tvz.tian-w.cn

[E13] 逐字符遍历
来源：http://edx.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://glf.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jqp.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://idn.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dch.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zlk.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lrw.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oen.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tlz.daria6918.cn

[E14] URL 编码与 Base64
来源：http://zkw.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hcg.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://vjs.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wuk.wangshuangyany.cn


<!-- 参考信息 -->