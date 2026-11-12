代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://idf.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lak.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tud.wangshuangyany.cn

[D06] 数组长度
来源：http://rqe.jianghu66.top

Py:   len(arr)
来源：http://ymv.vqdsnc.cn

PHP:  count($arr);
来源：http://oxs.bbcook.cn

JS:   arr.length
来源：http://ktw.shangyingyoupin.top

TS:   arr.length
来源：http://kcy.nanxuanxn.top

Java: list.size();
来源：http://nug.tanke756.top

Go:   len(arr)
来源：http://ovc.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://wmx.gotoacloud.top

C#:   list.Count;
来源：http://otw.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://qxt.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rle.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://eiw.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://gxs.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://tqo.iojbl.cn

Java: list.subList(1, 4);
来源：http://bid.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://moc.xuanzx.com

Ruby: arr[1, 3]
来源：http://xuy.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://knd.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://bmr.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://cfi.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://uta.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aqc.gzhubu.top

TS:   [...a, ...b];
来源：http://hoj.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgi.tarul.cn

Go:   append(a, b...)
来源：http://lxb.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://tfd.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://kod.9152youxi.cn

[D09] 排序（升序）
来源：http://ect.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://neh.yuxming.cn

PHP:  sort($arr);
来源：http://qsw.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cga.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wiv.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cfi.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jmu.sjlbkw.cn

Ruby: arr.sort
来源：http://vzy.jiagoushi.top

C#:   list.Sort();
来源：http://ypm.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rcf.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yhb.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lcj.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fny.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkj.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xet.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipe.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bro.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sjv.zhiwuduotai.top

[D11] 反转数组
来源：http://plm.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://lru.sxryk.cn

PHP:  array_reverse($arr);
来源：http://gxb.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dpa.daria6918.cn

TS:   [...arr].reverse();
来源：http://slo.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://utc.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://dpd.wangshuangyany.cn

Ruby: arr.reverse
来源：http://sna.chenjidiqi.icu

C#:   list.Reverse();
来源：http://nbz.shuidangran.top

[D12] 查找元素下标
来源：http://rxd.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://yps.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kpl.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aff.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzp.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wiz.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://xdz.hammf.cn

Ruby: arr.index(x)
来源：http://qxz.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://ijj.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://anl.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uzj.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rjo.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://wuf.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://kmv.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oie.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rsd.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://wuj.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://zls.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://sgw.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cmx.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kca.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://kxe.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://ymo.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://npc.havefunace.top

Go:   // 手写循环
来源：http://xvi.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://een.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rsg.hywenlv.cn

[D15] 去重
来源：http://van.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwk.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://sgw.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://dru.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://moi.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bpl.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://egp.xylfe.cn

Ruby: arr.uniq
来源：http://aqy.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://pno.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://tns.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://txf.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yir.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://byo.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jlz.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pci.gotoacloud.top

Go:   // 手写循环累加
来源：http://qsy.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jot.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://zod.9152youxi.cn

[D17] 最大值与最小值
来源：http://kwj.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://ylm.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://spm.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xxr.chenlongwang.top

TS:   Math.max(...arr);
来源：http://yen.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ayk.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oez.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://vte.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://imb.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://igj.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oiy.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://ddk.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hoi.zhiwuduotai.top

TS:   nested.flat();
来源：http://dlk.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pny.andypj.xyz

Go:   // 手写双层循环
来源：http://ram.epnwcf.com

Ruby: nested.flatten
来源：http://bwa.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://exb.cheryme.top

[D19] 按字段分组
来源：http://yaa.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://itf.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://egw.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqa.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zxv.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ngn.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://efp.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://yfr.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lmq.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://stl.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://tto.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://vxl.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwj.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sye.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mkc.fzhhl.top

Go:   // 手写 map[T]int
来源：http://cpi.gaohongyu789.top

Ruby: arr.tally
来源：http://yul.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://faz.tanke756.top

[D21] 判断是否包含某元素
来源：http://qoi.chenlongwang.top

Py:   x in arr
来源：http://dzi.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://xjc.guannengcc.top

JS:   arr.includes(x)
来源：http://wgn.andypj.xyz

TS:   arr.includes(x)
来源：http://zfy.yfazqb.com

Java: list.contains(x)
来源：http://auk.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://ahe.cdnleiting.top

Ruby: arr.include?(x)
来源：http://zgd.jyoumei.cn

C#:   list.Contains(x)
来源：http://zse.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://msn.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pyn.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evn.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qsd.cashguo.top

TS:   [...arr];
来源：http://whm.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://qzd.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vwc.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://ljz.andypj.xyz

C#:   new List<int>(list);
来源：http://pcr.tarul.cn

[D23] reduce 累积计算
来源：http://yfh.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tnm.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vvh.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jcd.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yxg.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://fbj.gzhubu.top

Go:   // 手写循环
来源：http://qxn.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vls.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rqv.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://wwb.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jna.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://utt.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hzm.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xmm.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dxz.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dhm.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://phh.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uzv.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://vki.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tah.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bhp.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://paj.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cdc.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uht.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tjs.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyf.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ymu.iojbl.cn

[D26] 数组转字符串
来源：http://ajj.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://hsp.meibo888.top

PHP:  implode(", ", $arr);
来源：http://gen.chenlongwang.top

JS:   arr.join(", ")
来源：http://kmx.aibaodan.cn

TS:   arr.join(", ")
来源：http://xhw.hnqzz.top

Java: String.join(", ", list)
来源：http://ydn.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://pxk.smart0.xyz

Ruby: arr.join(", ")
来源：http://zrs.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://xbt.shzxlz.cn

================================================================================
来源：http://fmx.zhengqikj.top

E. 字符串处理
来源：http://bwh.fanxiaobao.xyz

================================================================================
来源：http://wzt.guannengcc.top

[E01] 拼接字符串
来源：http://rkt.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uvo.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpc.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fyv.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://avm.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ibc.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://heq.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lmq.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ffs.vehdjk.com

[E02] 重复字符串
来源：http://mzx.zhijiandao.cn

Py:   "ab" * 3
来源：http://mno.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://sxk.yueranfly.top

JS:   "ab".repeat(3)
来源：http://zuu.smart0.xyz

TS:   "ab".repeat(3)
来源：http://nye.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://ttw.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://qdw.ctjpmb.com

Ruby: "ab" * 3
来源：http://ngh.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mro.yj20258888.top

[E03] 截取子串
来源：http://dcs.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lcz.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://efg.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kai.wangdashe.top

TS:   s.slice(1, 4)
来源：http://hlz.aibaodan.cn

Java: s.substring(1, 4)
来源：http://gpq.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhr.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://wfh.hammf.cn

C#:   s.Substring(1, 3)
来源：http://yxp.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://zny.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://qnl.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://qdh.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kln.nwbrower.top

TS:   s.indexOf("x")
来源：http://fdz.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://gwc.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://rhe.daria6918.cn

Ruby: s.index("x")
来源：http://dxx.sweek.top

C#:   s.IndexOf("x")
来源：http://cqs.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oxg.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xpi.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ing.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://heb.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rac.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfz.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nyv.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sxp.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ast.gogol.net.cn

[E06] 替换子串
来源：http://klx.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://odp.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://eyl.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qca.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://jgn.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhe.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mrr.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vbj.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://xzp.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://dln.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://msu.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pip.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tsg.hysaishi.cn

TS:   s.split(",")
来源：http://uzs.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ica.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pff.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://owf.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://igg.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://jiw.xziqi.cn

Py:   ",".join(items)
来源：http://jtk.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://hrn.yfazqb.com

JS:   items.join(",")
来源：http://fqk.yj20258888.top

TS:   items.join(",")
来源：http://ffb.zdbjq.cn

Java: String.join(",", items)
来源：http://uuf.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://fhz.zdbjq.cn

Ruby: items.join(",")
来源：http://cjs.haohaochexian.top

C#:   string.Join(",", items)
来源：http://fua.yueranfly.top

[E09] 去除所有空白字符
来源：http://xbq.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bhg.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vie.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://xth.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://tip.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://dsp.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vck.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qcz.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xau.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://mwf.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bkb.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yiu.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://sik.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://wal.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://hdz.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xma.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fes.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bxe.epnwcf.com

[E11] 反转字符串
来源：http://jns.haohaochexian.top

Py:   s[::-1]
来源：http://zpm.kuanghao11.cn

PHP:  strrev($s);
来源：http://sbx.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://cog.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://wkt.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qyi.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aqj.ybcxt.top

Ruby: s.reverse
来源：http://kmb.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://fil.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://ovj.wangdashe.top

Py:   s.count("a")
来源：http://hlo.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://hgw.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://qiv.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://bvv.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ctd.smart0.xyz


<!-- 参考信息 -->