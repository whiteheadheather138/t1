代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://rqg.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jvq.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfw.ppjwa.cn

[D06] 数组长度
来源：http://eei.ywan-chungtsiang.top

Py:   len(arr)
来源：http://fua.shuidangran.top

PHP:  count($arr);
来源：http://xcn.chenjidiqi.icu

JS:   arr.length
来源：http://zeu.ctjpmb.com

TS:   arr.length
来源：http://cqt.fktsv.cn

Java: list.size();
来源：http://dcf.316326.xyz

Go:   len(arr)
来源：http://eyv.bbcook.cn

Ruby: arr.length; arr.size
来源：http://kcf.ctjpmb.com

C#:   list.Count;
来源：http://izd.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://wke.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gfx.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zfk.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://mee.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://jvx.redwolf501.top

Java: list.subList(1, 4);
来源：http://rrq.fehbvm.com

Go:   arr[1:4]
来源：http://ubh.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://tvd.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://brw.pengpengdd.cyou

[D08] 合并两个数组
来源：http://ijv.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://njp.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://hcx.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://niy.daria6918.cn

TS:   [...a, ...b];
来源：http://gaw.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xhj.haohaochexian.top

Go:   append(a, b...)
来源：http://wnj.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://jlf.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://qwj.ivvv.top

[D09] 排序（升序）
来源：http://tyo.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://sdp.jlsjyb.cn

PHP:  sort($arr);
来源：http://eth.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uai.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bjk.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://siv.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://suh.shanyushiyangtech.top

Ruby: arr.sort
来源：http://pln.zhongyouzk.top

C#:   list.Sort();
来源：http://hnk.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uig.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tvh.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qwl.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xak.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qrl.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ghp.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://onm.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hzv.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jor.sjlbkw.cn

[D11] 反转数组
来源：http://gsc.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://rfp.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://htj.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://chp.yuxming.cn

TS:   [...arr].reverse();
来源：http://pbt.tarul.cn

Java: Collections.reverse(list);
来源：http://jvl.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://ywo.ehwqpu.com

Ruby: arr.reverse
来源：http://vgh.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://mus.yuxming.cn

[D12] 查找元素下标
来源：http://xdt.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://ewv.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fvw.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xqk.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://whj.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kxj.tanke756.top

Go:   slices.Index(arr, x)
来源：http://bqm.pycfn.com

Ruby: arr.index(x)
来源：http://vae.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://tff.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://aaa.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjz.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://meb.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://dhx.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://ilv.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nvh.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vlz.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://cxn.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eev.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://wkg.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ekg.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://utf.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://bmy.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://sra.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xov.xuanzx.com

Go:   // 手写循环
来源：http://xhb.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yxh.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sdt.hnxiangtu.top

[D15] 去重
来源：http://kje.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ypv.guannengcc.top

PHP:  array_unique($arr);
来源：http://qvl.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://tca.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://uab.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://met.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://fjp.cashguo.top

Ruby: arr.uniq
来源：http://fwx.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://jvm.gzhubu.top

[D16] 求和与平均值
来源：http://zjd.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cfq.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ybm.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sob.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fpu.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qmf.hesvh.cn

Go:   // 手写循环累加
来源：http://zbl.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wuw.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://ssy.gogol.net.cn

[D17] 最大值与最小值
来源：http://ebe.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://pdk.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://jtt.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bub.shzxlz.cn

TS:   Math.max(...arr);
来源：http://cda.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qpc.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gjj.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://ebt.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://baq.birdmap.top

[D18] 扁平化嵌套数组
来源：http://sig.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mid.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://ptb.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lie.hcnkem.com

TS:   nested.flat();
来源：http://knp.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pyp.hfpthk.cn

Go:   // 手写双层循环
来源：http://fxy.fengsongda.top

Ruby: nested.flatten
来源：http://gez.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fno.vqdsnc.cn

[D19] 按字段分组
来源：http://bhk.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ufi.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bzk.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://toz.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aie.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jxc.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://vyi.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://msh.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rul.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://xdv.tian-w.cn

Py:   Counter(arr)
来源：http://ogy.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://pre.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ort.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pie.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mdy.mhx1999.top

Go:   // 手写 map[T]int
来源：http://vtp.yuanzhike.top

Ruby: arr.tally
来源：http://orj.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yku.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://pnn.sysykeji.top

Py:   x in arr
来源：http://cwt.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://obn.tian-w.cn

JS:   arr.includes(x)
来源：http://odm.yj20258.top

TS:   arr.includes(x)
来源：http://bng.52xcode.cn

Java: list.contains(x)
来源：http://ynl.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://oba.zhixingplan.top

Ruby: arr.include?(x)
来源：http://xrn.nanxuanxn.top

C#:   list.Contains(x)
来源：http://taj.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://cvt.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mxk.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rvz.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://moa.hnxiangtu.top

TS:   [...arr];
来源：http://lpa.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://oeq.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://njr.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://rhp.jinqigfzy.top

C#:   new List<int>(list);
来源：http://qwo.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://opf.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dox.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lwe.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svx.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://phw.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fox.yanxiufei.cn

Go:   // 手写循环
来源：http://jds.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fad.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tij.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://veb.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cph.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://niy.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zfb.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vnq.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://err.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewj.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jdw.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nst.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://bun.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bph.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nme.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cic.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tlf.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kdn.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cdz.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sku.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ecq.yuanzhike.top

[D26] 数组转字符串
来源：http://kwu.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://dla.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://aug.guowangkeji.top

JS:   arr.join(", ")
来源：http://sfd.hywenlv.cn

TS:   arr.join(", ")
来源：http://nsb.aibaodan.cn

Java: String.join(", ", list)
来源：http://fap.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://ncz.redwolf501.top

Ruby: arr.join(", ")
来源：http://iir.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://fca.zhongyouzk.top

================================================================================
来源：http://rfv.ybcxt.top

E. 字符串处理
来源：http://qak.zhaomingkeji.xyz

================================================================================
来源：http://dqd.zdbjq.cn

[E01] 拼接字符串
来源：http://hte.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gwp.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fue.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kqn.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wil.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://krm.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sbw.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tej.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yey.cheryme.top

[E02] 重复字符串
来源：http://bwv.hnxiangtu.top

Py:   "ab" * 3
来源：http://yca.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://ugx.daxiang520.top

JS:   "ab".repeat(3)
来源：http://bgi.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://jtq.jiagoushi.top

Java: "ab".repeat(3)
来源：http://qqz.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://bqm.hesvh.cn

Ruby: "ab" * 3
来源：http://stw.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zns.yj20258888.top

[E03] 截取子串
来源：http://omq.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nhp.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jlx.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oiu.fktsv.cn

TS:   s.slice(1, 4)
来源：http://qsg.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://bts.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://grm.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://fkx.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://agw.sweek.top

[E04] 查找子串位置
来源：http://vkk.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://ypt.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://yzw.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ept.gogol.net.cn

TS:   s.indexOf("x")
来源：http://fzt.yuanzhike.top

Java: s.indexOf("x")
来源：http://ezr.tanke756.top

Go:   strings.Index(s, "x")
来源：http://kcu.iojbl.cn

Ruby: s.index("x")
来源：http://giw.smart0.xyz

C#:   s.IndexOf("x")
来源：http://ckq.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mng.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cma.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gqu.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqm.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mlw.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szm.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jtu.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hmn.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thg.zdbjq.cn

[E06] 替换子串
来源：http://fsc.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nsl.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://tnf.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lps.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://mxg.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sjj.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://znp.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://twp.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://wfe.hammf.cn

[E07] 按分隔符拆分
来源：http://gau.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://syl.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://osm.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wun.hnxiangtu.top

TS:   s.split(",")
来源：http://een.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vzj.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zgo.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://rwb.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zjz.shuidangran.top

[E08] 数组按分隔符合并
来源：http://ddj.hysaishi.cn

Py:   ",".join(items)
来源：http://pkj.xinyue.icu

PHP:  implode(",", $items);
来源：http://yla.zhijiandao.cn

JS:   items.join(",")
来源：http://rmk.aibaodan.cn

TS:   items.join(",")
来源：http://peg.hywenlv.cn

Java: String.join(",", items)
来源：http://ivk.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://zxj.vqdsnc.cn

Ruby: items.join(",")
来源：http://qoo.hammf.cn

C#:   string.Join(",", items)
来源：http://iij.smart0.xyz

[E09] 去除所有空白字符
来源：http://xoi.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mmw.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blu.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://cjd.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://rar.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://vus.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://unr.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://skw.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yaz.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://unn.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpz.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ffw.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://flo.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://nfy.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://tof.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://yfk.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xav.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jrr.shangyingyoupin.top

[E11] 反转字符串
来源：http://lpr.xylfe.cn

Py:   s[::-1]
来源：http://gjw.hysaishi.cn

PHP:  strrev($s);
来源：http://uak.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://nfx.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://euv.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ven.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tua.yj202588.top

Ruby: s.reverse
来源：http://jbz.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yiv.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://dfx.uphjek.com

Py:   s.count("a")
来源：http://dig.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://yzo.yj202588.top

JS:   s.split("a").length - 1
来源：http://poo.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://avo.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ipm.nanxuanxn.top


<!-- 参考信息 -->