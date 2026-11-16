代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jjc.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fxf.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://zwi.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://rrg.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://irn.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mry.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uwq.daxiang520.top

[D06] 数组长度
来源：http://anf.nwbrower.top

Py:   len(arr)
来源：http://amd.ydzc1.top

PHP:  count($arr);
来源：http://sew.ydzc1.top

JS:   arr.length
来源：http://led.yvedp.cn

TS:   arr.length
来源：http://dyq.hysaishi.cn

Java: list.size();
来源：http://vlm.c1oappe.top

Go:   len(arr)
来源：http://vcp.uphjek.com

Ruby: arr.length; arr.size
来源：http://olt.guannengcc.top

C#:   list.Count;
来源：http://uti.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://kvn.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zxu.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gev.havefunace.top

JS:   arr.slice(1, 4);
来源：http://frp.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://itu.sxryk.cn

Java: list.subList(1, 4);
来源：http://gok.meibo888.top

Go:   arr[1:4]
来源：http://smr.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://vdx.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://vqw.chenlongwang.top

[D08] 合并两个数组
来源：http://fvf.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://isy.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://sbk.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mow.birdmap.top

TS:   [...a, ...b];
来源：http://sdl.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eng.zdqjudy.top

Go:   append(a, b...)
来源：http://rbr.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://oov.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://fbt.cucudq.cn

[D09] 排序（升序）
来源：http://vvs.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://tci.hongshengwenyu.top

PHP:  sort($arr);
来源：http://phu.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uec.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://onr.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uqp.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xti.fzhhl.top

Ruby: arr.sort
来源：http://yyu.cdnleiting.top

C#:   list.Sort();
来源：http://mxt.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hen.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hls.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ttk.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jce.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhw.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://inb.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uvk.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://amq.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qkx.hongshengwenyu.top

[D11] 反转数组
来源：http://juv.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://rkw.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://noy.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fow.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://xtl.guowangkeji.top

Java: Collections.reverse(list);
来源：http://pxd.yonumen.top

Go:   slices.Reverse(arr)
来源：http://gai.nanxuanxn.top

Ruby: arr.reverse
来源：http://jtg.yueranfly.top

C#:   list.Reverse();
来源：http://wva.tianlin.xyz

[D12] 查找元素下标
来源：http://pys.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://roy.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cim.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rhf.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nrs.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mfz.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://rlr.zhengqikj.top

Ruby: arr.index(x)
来源：http://jac.tian-w.cn

C#:   list.IndexOf(x);
来源：http://uzb.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://lza.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rmq.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vid.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://jmr.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://mcv.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://doq.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cgl.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qpt.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://utd.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://bwb.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pcw.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vho.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://kum.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://atw.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dhn.fanxiaobao.xyz

Go:   // 手写循环
来源：http://vtl.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hiu.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tfj.ctjpmb.com

[D15] 去重
来源：http://lim.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xiv.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://qdr.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://cem.shangyingyoupin.top

TS:   [...new Set(arr)]
来源：http://vnj.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lpy.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ftt.hywenlv.cn

Ruby: arr.uniq
来源：http://nsn.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://nlb.aizwys.cn

[D16] 求和与平均值
来源：http://sxm.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qoe.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wlc.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://drm.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjj.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eah.uphjek.com

Go:   // 手写循环累加
来源：http://jrc.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ggc.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://sfa.vqdsnc.cn

[D17] 最大值与最小值
来源：http://vty.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://auj.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://bqo.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ybo.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://cwj.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mkd.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wiy.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://gka.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://vsv.havefunace.top

[D18] 扁平化嵌套数组
来源：http://rgq.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wzo.sweek.top

PHP:  array_merge(...$nested);
来源：http://yju.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://btr.bbcook.cn

TS:   nested.flat();
来源：http://icf.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vpc.zhijiandao.cn

Go:   // 手写双层循环
来源：http://jcb.dashuyun.cn

Ruby: nested.flatten
来源：http://mop.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jpp.yj202588.top

[D19] 按字段分组
来源：http://cpw.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xax.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bti.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fyu.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xnw.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vmo.havefunace.top

Go:   // 手写 map[string][]T
来源：http://dau.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwd.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gfr.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://kke.xylfe.cn

Py:   Counter(arr)
来源：http://ono.yuxming.cn

PHP:  array_count_values($arr);
来源：http://ylt.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ial.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fva.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://udy.bjfxy.top

Go:   // 手写 map[T]int
来源：http://rqs.vqdsnc.cn

Ruby: arr.tally
来源：http://twd.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nnn.ybcxt.top

[D21] 判断是否包含某元素
来源：http://lnj.sjlbkw.cn

Py:   x in arr
来源：http://gjk.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://tfi.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://xcd.yanxiufei.cn

TS:   arr.includes(x)
来源：http://qrz.dashuyun.cn

Java: list.contains(x)
来源：http://sot.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://jnv.fengsongda.top

Ruby: arr.include?(x)
来源：http://bez.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://jqw.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://yvo.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xxm.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ene.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eui.0kj1m.cn

TS:   [...arr];
来源：http://zxc.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://oir.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yfv.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://zwg.yuxming.cn

C#:   new List<int>(list);
来源：http://gbc.vqdsnc.cn

[D23] reduce 累积计算
来源：http://lvf.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://urj.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bnz.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvl.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fop.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zkt.kuanghao11.cn

Go:   // 手写循环
来源：http://kqv.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gxo.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eud.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://gef.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ghb.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xrt.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bym.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zjc.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cft.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yyb.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ajn.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aww.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://pqg.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bwd.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cpo.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xoo.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://agd.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tnu.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mlg.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kpm.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jfg.zhiwuduotai.top

[D26] 数组转字符串
来源：http://eei.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://kfk.hammf.cn

PHP:  implode(", ", $arr);
来源：http://vfo.fehbvm.com

JS:   arr.join(", ")
来源：http://xjd.jlsjyb.cn

TS:   arr.join(", ")
来源：http://zgv.zycfv.cn

Java: String.join(", ", list)
来源：http://cfl.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://evy.cdnleiting.top

Ruby: arr.join(", ")
来源：http://oma.c1oappe.top

C#:   string.Join(", ", list)
来源：http://gie.yfazqb.com

================================================================================
来源：http://uqu.fengsongda.top

E. 字符串处理
来源：http://npw.xingfuxueyuan.xyz

================================================================================
来源：http://pnf.meibo888.top

[E01] 拼接字符串
来源：http://eol.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jli.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byl.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://osl.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jnc.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cvq.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://auj.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sch.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ozw.zycfv.cn

[E02] 重复字符串
来源：http://wpu.jqgufenzy.top

Py:   "ab" * 3
来源：http://mvk.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://cqz.guannengcc.top

JS:   "ab".repeat(3)
来源：http://xxj.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://cyi.xuanzx.com

Java: "ab".repeat(3)
来源：http://gho.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://qsg.c1oappe.top

Ruby: "ab" * 3
来源：http://psx.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qkt.zhaomingkeji.xyz

[E03] 截取子串
来源：http://paf.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hva.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tvd.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csp.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://vut.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://juu.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xwf.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://knz.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://qij.tianlin.xyz

[E04] 查找子串位置
来源：http://guq.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://epp.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://puq.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ruw.gogol.net.cn

TS:   s.indexOf("x")
来源：http://mdm.9152youxi.cn

Java: s.indexOf("x")
来源：http://cbf.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://ovc.guannengcc.top

Ruby: s.index("x")
来源：http://wmf.sysykeji.top

C#:   s.IndexOf("x")
来源：http://cmo.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xxu.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wli.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yxm.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgr.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gkg.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmz.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zsb.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bod.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nia.tanke756.top

[E06] 替换子串
来源：http://zvd.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dwb.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://qxk.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pln.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://svx.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lei.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mog.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gmf.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://onh.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://ygn.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xvf.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://swt.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wcf.aibaodan.cn

TS:   s.split(",")
来源：http://xyd.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://dcv.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hhy.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://nbz.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hvl.sysykeji.top

[E08] 数组按分隔符合并
来源：http://sky.nanxinkj.top

Py:   ",".join(items)
来源：http://xnx.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://vsy.cashguo.top

JS:   items.join(",")
来源：http://der.nanxinkj.top

TS:   items.join(",")
来源：http://jyb.yuanzhike.top

Java: String.join(",", items)
来源：http://xoy.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://pob.zhixingplan.top

Ruby: items.join(",")
来源：http://xeo.sxryk.cn

C#:   string.Join(",", items)
来源：http://yeu.xylfe.cn

[E09] 去除所有空白字符
来源：http://hzx.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zfy.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nyv.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://ioz.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://fzv.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://pun.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rau.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://xea.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsh.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://wii.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jhj.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zkd.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://zpt.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://fvq.yuxming.cn

Java: String.format("%03d", 7)
来源：http://rxn.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://elk.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://otq.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eez.fengsongda.top

[E11] 反转字符串
来源：http://vwq.chenjidiqi.icu

Py:   s[::-1]
来源：http://yaz.hnqzz.top

PHP:  strrev($s);
来源：http://jmp.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://huf.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://dkt.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://srp.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://huz.9152youxi.cn

Ruby: s.reverse
来源：http://lfh.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jbw.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://moz.hnxiangtu.top

Py:   s.count("a")
来源：http://lxz.svipenyu.cn


<!-- 参考信息 -->