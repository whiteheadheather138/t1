代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dcn.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yjh.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://pyk.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://duq.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ddc.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://net.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ari.zhixingplan.top

[D06] 数组长度
来源：http://azk.snrcjt.cn

Py:   len(arr)
来源：http://jae.havefunace.top

PHP:  count($arr);
来源：http://fvn.zycfv.cn

JS:   arr.length
来源：http://wwz.shangyingyoupin.top

TS:   arr.length
来源：http://grl.xziqi.cn

Java: list.size();
来源：http://xlf.wangdashe.top

Go:   len(arr)
来源：http://hxv.yvedp.cn

Ruby: arr.length; arr.size
来源：http://mkf.yanxiufei.cn

C#:   list.Count;
来源：http://drl.52xcode.cn

[D07] 切片 / 取子数组
来源：http://oyz.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://apr.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://iad.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://kce.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://sim.jinqigufen.top

Java: list.subList(1, 4);
来源：http://wgw.ydjk.org.cn

Go:   arr[1:4]
来源：http://jrt.tianlin.xyz

Ruby: arr[1, 3]
来源：http://jyz.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://bwu.yuxming.cn

[D08] 合并两个数组
来源：http://sdk.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://pyn.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://znr.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://muk.daxiang520.top

TS:   [...a, ...b];
来源：http://zcy.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ske.hesvh.cn

Go:   append(a, b...)
来源：http://rrn.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://kij.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://qdo.haohaochexian.top

[D09] 排序（升序）
来源：http://yca.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://udo.hammf.cn

PHP:  sort($arr);
来源：http://tqj.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uck.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://cja.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zux.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aqr.jinghuilouyu.cn

Ruby: arr.sort
来源：http://jie.daria6918.cn

C#:   list.Sort();
来源：http://jrl.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mxi.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ebf.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqt.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jlw.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngc.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://umc.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dxf.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://csw.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://owz.chenlongwang.top

[D11] 反转数组
来源：http://aff.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://pxu.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://uud.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ned.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://yfm.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://miq.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://ceb.yvedp.cn

Ruby: arr.reverse
来源：http://yig.nanxinkj.top

C#:   list.Reverse();
来源：http://lvi.yangfankeji.com

[D12] 查找元素下标
来源：http://fmb.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://czx.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lif.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgq.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://puj.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pmz.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://oyd.dashuyun.cn

Ruby: arr.index(x)
来源：http://zhm.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://cwm.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://dbu.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gmj.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dyf.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://yql.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://qdl.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bqs.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfb.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://mhk.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mbk.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://jnh.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zqh.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dox.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://iht.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://oyb.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://voy.xuetiantiany.cn

Go:   // 手写循环
来源：http://uba.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mqk.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qdq.sweek.top

[D15] 去重
来源：http://bwh.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://psp.iojbl.cn

PHP:  array_unique($arr);
来源：http://cqt.hcnkem.com

JS:   [...new Set(arr)]
来源：http://uuz.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://vxi.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ior.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fpk.yj20258.top

Ruby: arr.uniq
来源：http://kwy.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://nza.kuanghao11.cn

[D16] 求和与平均值
来源：http://ynm.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fxg.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nae.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qph.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgs.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://idy.hnqzz.top

Go:   // 手写循环累加
来源：http://hfv.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lws.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://dtm.meibo888.top

[D17] 最大值与最小值
来源：http://etc.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://mml.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://acf.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://paz.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://drs.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zpu.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jxw.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://jij.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://lgf.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://gcq.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wvi.cheryme.top

PHP:  array_merge(...$nested);
来源：http://gzo.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cwi.cqqwz.cn

TS:   nested.flat();
来源：http://nkn.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://euu.zhoulong.xyz

Go:   // 手写双层循环
来源：http://qqo.svipenyu.cn

Ruby: nested.flatten
来源：http://xvj.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yhf.sxryk.cn

[D19] 按字段分组
来源：http://mvz.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rbt.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rcb.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qnp.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qyw.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lkw.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://uzc.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://myt.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://teu.havefunace.top

[D20] 统计每个元素出现次数
来源：http://sdm.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://cel.cheryme.top

PHP:  array_count_values($arr);
来源：http://whh.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vor.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euj.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://adu.xziqi.cn

Go:   // 手写 map[T]int
来源：http://eoa.guannengcc.top

Ruby: arr.tally
来源：http://zdo.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rhf.c1oappe.top

[D21] 判断是否包含某元素
来源：http://agt.52xcode.cn

Py:   x in arr
来源：http://ksy.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://mgl.svipenyu.cn

JS:   arr.includes(x)
来源：http://qjb.xuanzx.com

TS:   arr.includes(x)
来源：http://ltk.jyoumei.cn

Java: list.contains(x)
来源：http://iln.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://rwd.fzhhl.top

Ruby: arr.include?(x)
来源：http://lbd.zhongyouzk.top

C#:   list.Contains(x)
来源：http://bhs.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://mck.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zed.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ade.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://itk.havefunace.top

TS:   [...arr];
来源：http://fvv.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://plc.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://auk.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://bkl.sysykeji.top

C#:   new List<int>(list);
来源：http://mfc.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://fbu.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yrz.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mqd.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abf.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bio.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mpq.birdmap.top

Go:   // 手写循环
来源：http://pzj.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yxr.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ppd.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://jka.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rjm.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsv.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myc.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hxo.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zqe.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xos.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gau.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xhy.tarul.cn

[D25] Set 集合去重与交并差
来源：http://wxi.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tcz.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ztj.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nbi.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fqy.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wma.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jjo.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezw.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://edu.jlsjyb.cn

[D26] 数组转字符串
来源：http://ktt.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://fin.cashguo.top

PHP:  implode(", ", $arr);
来源：http://qzc.haohaochexian.top

JS:   arr.join(", ")
来源：http://lqz.pycfn.com

TS:   arr.join(", ")
来源：http://lih.cheryme.top

Java: String.join(", ", list)
来源：http://gya.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://xab.uphjek.com

Ruby: arr.join(", ")
来源：http://quu.sweek.top

C#:   string.Join(", ", list)
来源：http://xby.jyoumei.cn

================================================================================
来源：http://uun.dianchejie.cn

E. 字符串处理
来源：http://wty.fktsv.cn

================================================================================
来源：http://xhg.xuanzx.com

[E01] 拼接字符串
来源：http://teu.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jaa.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oqe.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://itl.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbg.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pey.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://glw.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yit.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgh.shangyingyoupin.top

[E02] 重复字符串
来源：http://qns.meibo888.top

Py:   "ab" * 3
来源：http://zre.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://kvi.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://fuj.havefunace.top

TS:   "ab".repeat(3)
来源：http://fiw.nwbrower.top

Java: "ab".repeat(3)
来源：http://oew.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://wer.hfpthk.cn

Ruby: "ab" * 3
来源：http://bim.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aac.yj202588.top

[E03] 截取子串
来源：http://cis.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zsf.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fyv.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ity.fzhhl.top

TS:   s.slice(1, 4)
来源：http://tbh.aibaodan.cn

Java: s.substring(1, 4)
来源：http://nbh.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ozj.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://muz.cheryme.top

C#:   s.Substring(1, 3)
来源：http://gew.yuxming.cn

[E04] 查找子串位置
来源：http://fyf.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://ctj.xuanzx.com

PHP:  strpos($s, "x");
来源：http://yjh.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lhv.yvedp.cn

TS:   s.indexOf("x")
来源：http://cyd.zycfv.cn

Java: s.indexOf("x")
来源：http://bea.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://iku.smart0.xyz

Ruby: s.index("x")
来源：http://mng.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://rzr.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pvo.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hwo.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eep.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptw.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://lno.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fdv.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajc.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lix.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kgj.tian-w.cn

[E06] 替换子串
来源：http://zrc.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sdh.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://vyo.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zwt.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://bmz.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://esx.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://flp.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eyl.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://tal.yonumen.top

[E07] 按分隔符拆分
来源：http://vxh.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://phv.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tjz.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yxk.jqgfzy.top

TS:   s.split(",")
来源：http://kzq.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://flh.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lqg.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://oxh.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tke.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://ivf.dashuyun.cn

Py:   ",".join(items)
来源：http://auv.hfpthk.cn

PHP:  implode(",", $items);
来源：http://geh.ehwqpu.com

JS:   items.join(",")
来源：http://dkz.andypj.xyz

TS:   items.join(",")
来源：http://xuw.snrcjt.cn

Java: String.join(",", items)
来源：http://vrv.cashguo.top

Go:   strings.Join(items, ",")
来源：http://mzg.yj202588.top

Ruby: items.join(",")
来源：http://rab.0kj1m.cn

C#:   string.Join(",", items)
来源：http://lnx.ppjwa.cn

[E09] 去除所有空白字符
来源：http://iiq.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ncd.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xmo.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://wvj.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://uem.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://nbq.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yxs.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://spu.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yoi.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://agb.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mtj.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jta.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://feg.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://ely.xylfe.cn

Java: String.format("%03d", 7)
来源：http://nnw.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zko.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udz.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jvr.tian-w.cn

[E11] 反转字符串
来源：http://rfz.yonumen.top

Py:   s[::-1]
来源：http://xqh.xuanzx.com

PHP:  strrev($s);
来源：http://ove.havefunace.top

JS:   [...s].reverse().join("")
来源：http://drp.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://ahd.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pzu.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qck.ivvv.top

Ruby: s.reverse
来源：http://dqx.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://agu.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://vjn.zdbjq.cn

Py:   s.count("a")
来源：http://wnj.xuanzx.com


<!-- 参考信息 -->