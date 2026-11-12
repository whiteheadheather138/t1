代发 wailian999

TS:   arr.slice(1, 4);
来源：http://rvg.xziqi.cn

Java: list.subList(1, 4);
来源：http://kgg.gogol.net.cn

Go:   arr[1:4]
来源：http://vzj.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://wjf.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://nfv.sweek.top

[D08] 合并两个数组
来源：http://mbc.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://gmu.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://qer.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cre.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://dwy.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kbl.xinyue.icu

Go:   append(a, b...)
来源：http://ghm.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://cje.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://znx.gotoacloud.top

[D09] 排序（升序）
来源：http://hyg.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://kfm.ppjwa.cn

PHP:  sort($arr);
来源：http://kvx.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dwo.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vtj.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lev.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xnd.feifeiyinyue.top

Ruby: arr.sort
来源：http://bgk.daria6918.cn

C#:   list.Sort();
来源：http://uey.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://jel.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pvz.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ilc.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nze.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujt.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uan.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fil.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sbw.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rqq.zhoulong.xyz

[D11] 反转数组
来源：http://bdj.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://kcc.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://lsr.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vko.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://nqb.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://eei.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://gix.uphjek.com

Ruby: arr.reverse
来源：http://iec.jqgufenzy.top

C#:   list.Reverse();
来源：http://faf.ctjpmb.com

[D12] 查找元素下标
来源：http://mct.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://kqw.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vex.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sju.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xzm.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kjy.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://fsq.9152youxi.cn

Ruby: arr.index(x)
来源：http://cla.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://ykc.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://laf.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yeo.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bko.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://nty.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://qkq.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qgj.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://isn.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cfx.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jcx.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://jth.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fme.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aay.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://qbh.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://dzh.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ffj.gogol.net.cn

Go:   // 手写循环
来源：http://vbk.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://ijg.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dek.xuetiantiany.cn

[D15] 去重
来源：http://pyi.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ota.daria6918.cn

PHP:  array_unique($arr);
来源：http://uxx.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://xpa.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://uja.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ymz.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://dfr.sysykeji.top

Ruby: arr.uniq
来源：http://ota.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://kxo.sjlbkw.cn

[D16] 求和与平均值
来源：http://efe.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nkz.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sqn.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcq.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xnq.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fdu.bbcook.cn

Go:   // 手写循环累加
来源：http://prj.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ive.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://mbv.zycfv.cn

[D17] 最大值与最小值
来源：http://jnz.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://shl.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://efm.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzz.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://das.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sbd.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zwh.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://qqx.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://xqw.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://sar.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://czq.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://trz.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oii.hesvh.cn

TS:   nested.flat();
来源：http://yur.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dxj.pycfn.com

Go:   // 手写双层循环
来源：http://nkb.sxryk.cn

Ruby: nested.flatten
来源：http://etk.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://icv.316326.xyz

[D19] 按字段分组
来源：http://dmp.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qah.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ivx.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hfe.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jfs.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aey.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://rhr.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rxg.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xse.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://nyp.andypj.xyz

Py:   Counter(arr)
来源：http://iog.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://cez.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvc.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bsz.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gir.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://soq.zhengqikj.top

Ruby: arr.tally
来源：http://hjs.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qty.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://upi.yangfankeji.com

Py:   x in arr
来源：http://bdq.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://cjt.c1oappe.top

JS:   arr.includes(x)
来源：http://igc.jinqigufen.top

TS:   arr.includes(x)
来源：http://lfy.chenlongwang.top

Java: list.contains(x)
来源：http://amw.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://ovq.bjfxy.top

Ruby: arr.include?(x)
来源：http://mqc.yfazqb.com

C#:   list.Contains(x)
来源：http://ybq.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://kox.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kym.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlm.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gtx.zycfv.cn

TS:   [...arr];
来源：http://qjw.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://bis.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://yce.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://gow.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://jgk.yj20258.top

[D23] reduce 累积计算
来源：http://tip.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wwv.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mpx.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncr.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nif.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qqz.quarkkingdee.top

Go:   // 手写循环
来源：http://ssg.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pfs.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oen.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://shl.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rps.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://feo.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bsa.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pre.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lrg.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eba.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yxq.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mwf.tanke756.top

[D25] Set 集合去重与交并差
来源：http://kag.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gfq.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qhg.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qbj.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gcm.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hdm.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xld.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gue.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://txg.cheryme.top

[D26] 数组转字符串
来源：http://baj.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://voc.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://fmn.wangdashe.top

JS:   arr.join(", ")
来源：http://dqp.316326.xyz

TS:   arr.join(", ")
来源：http://hmp.xylfe.cn

Java: String.join(", ", list)
来源：http://hdb.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://nsi.jqgfzy.top

Ruby: arr.join(", ")
来源：http://fyz.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://ags.xuanzx.com

================================================================================
来源：http://lwy.yonumen.top

E. 字符串处理
来源：http://jiy.fzhhl.top

================================================================================
来源：http://bvx.svipenyu.cn

[E01] 拼接字符串
来源：http://ijb.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mru.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vqz.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxo.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nos.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xqq.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://awh.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zdu.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://poi.ydzc1.top

[E02] 重复字符串
来源：http://een.zhongyouzk.top

Py:   "ab" * 3
来源：http://ofi.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://vad.fktsv.cn

JS:   "ab".repeat(3)
来源：http://xdb.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://cjl.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://fsv.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://qqy.svipenyu.cn

Ruby: "ab" * 3
来源：http://fxt.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsa.cdnleiting.top

[E03] 截取子串
来源：http://oqn.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yny.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://amt.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pcx.yvedp.cn

TS:   s.slice(1, 4)
来源：http://ghp.hfpthk.cn

Java: s.substring(1, 4)
来源：http://swp.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://isg.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://mjn.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://rhj.fengsongda.top

[E04] 查找子串位置
来源：http://wkg.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://lzr.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://xqr.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://top.fzhhl.top

TS:   s.indexOf("x")
来源：http://ugu.cucudq.cn

Java: s.indexOf("x")
来源：http://rig.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://rze.yfazqb.com

Ruby: s.index("x")
来源：http://vlo.epnwcf.com

C#:   s.IndexOf("x")
来源：http://bja.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywn.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://odj.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cqh.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ish.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://shk.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ssj.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xxo.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kxs.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://num.vqdsnc.cn

[E06] 替换子串
来源：http://dlg.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fix.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ezf.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yis.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://qfr.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nio.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://chl.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ite.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://kso.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://tiq.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://grf.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zsm.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aie.xinyue.icu

TS:   s.split(",")
来源：http://qdp.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://agp.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qva.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://lfv.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ili.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://epo.zhongyouzk.top

Py:   ",".join(items)
来源：http://qog.xuanzx.com

PHP:  implode(",", $items);
来源：http://ytt.xziqi.cn

JS:   items.join(",")
来源：http://ycv.cheryme.top

TS:   items.join(",")
来源：http://vpw.andypj.xyz

Java: String.join(",", items)
来源：http://bcs.uphjek.com

Go:   strings.Join(items, ",")
来源：http://osc.hywenlv.cn

Ruby: items.join(",")
来源：http://nfn.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://pam.hammf.cn

[E09] 去除所有空白字符
来源：http://tpn.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://crp.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cjs.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://ysd.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://sno.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ryf.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qjw.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ioe.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wst.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://yiv.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spu.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qnf.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://ewi.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://xal.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://gpn.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qls.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esh.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ypq.jqgufenzy.top

[E11] 反转字符串
来源：http://jqd.hesvh.cn

Py:   s[::-1]
来源：http://zdp.sweek.top

PHP:  strrev($s);
来源：http://yre.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://rih.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://ahy.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://boc.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gqa.pycfn.com

Ruby: s.reverse
来源：http://nba.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rdg.bbcook.cn

[E12] 统计某字符出现次数
来源：http://phk.sjlbkw.cn

Py:   s.count("a")
来源：http://vdr.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://ftx.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://eud.cashguo.top

TS:   s.split("a").length - 1
来源：http://ptc.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aie.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ems.xylfe.cn

Ruby: s.count("a")
来源：http://lug.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://mst.havefunace.top

[E13] 逐字符遍历
来源：http://she.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://bqh.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sxu.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ffi.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sro.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kgx.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jtg.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://evv.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wxb.fktsv.cn

[E14] URL 编码与 Base64
来源：http://kqk.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pnr.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nhg.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojs.quarkkingdee.top


<!-- 参考信息 -->