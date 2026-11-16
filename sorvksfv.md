代发 wailian999

PHP:  sort($arr);
来源：http://ceu.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uyw.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbe.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://opo.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lqi.yfazqb.com

Ruby: arr.sort
来源：http://deo.jiagoushi.top

C#:   list.Sort();
来源：http://dqo.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bla.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uhu.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://trg.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bpy.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndb.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uzx.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vjl.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eye.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lmr.vehdjk.com

[D11] 反转数组
来源：http://bsp.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://fwg.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://vmr.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eap.yueranfly.top

TS:   [...arr].reverse();
来源：http://nts.hywenlv.cn

Java: Collections.reverse(list);
来源：http://igk.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://rcp.gaohongyu789.top

Ruby: arr.reverse
来源：http://quv.cashguo.top

C#:   list.Reverse();
来源：http://ddl.chenzaomai.com

[D12] 查找元素下标
来源：http://sjj.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://tna.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://idh.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lkr.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://moq.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rvo.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://pau.iojbl.cn

Ruby: arr.index(x)
来源：http://rjz.yfazqb.com

C#:   list.IndexOf(x);
来源：http://ovh.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://iku.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gjh.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wof.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://ijh.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://hjy.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cxv.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ldc.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://vak.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vmb.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://itf.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cxp.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhf.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://whu.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://uev.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hml.pengpengdd.cyou

Go:   // 手写循环
来源：http://wik.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://npt.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ikl.redwolf501.top

[D15] 去重
来源：http://kfy.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dmf.hfpthk.cn

PHP:  array_unique($arr);
来源：http://foc.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://xmc.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://ipa.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vzx.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hba.tian-w.cn

Ruby: arr.uniq
来源：http://izi.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://ckg.nwbrower.top

[D16] 求和与平均值
来源：http://exv.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vlh.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gqp.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://crv.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzv.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://djx.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://gsb.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqa.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://ebt.hcnkem.com

[D17] 最大值与最小值
来源：http://lgx.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://osc.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://tym.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hlb.yj20258.top

TS:   Math.max(...arr);
来源：http://xrj.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gcx.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nxw.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://ohk.cheryme.top

C#:   list.Max();  list.Min()
来源：http://qab.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://niq.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tkp.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://mip.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xow.yuxming.cn

TS:   nested.flat();
来源：http://noq.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wdc.zhixingplan.top

Go:   // 手写双层循环
来源：http://lqj.hfpthk.cn

Ruby: nested.flatten
来源：http://vfg.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nll.hfpthk.cn

[D19] 按字段分组
来源：http://xwm.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://luo.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rks.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hit.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ygu.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fac.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://eag.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://muu.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxf.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://gjf.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://xdf.gzhubu.top

PHP:  array_count_values($arr);
来源：http://ckc.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jar.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bry.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ect.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://tyx.jlsjyb.cn

Ruby: arr.tally
来源：http://vbi.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufy.tian-w.cn

[D21] 判断是否包含某元素
来源：http://sns.yuanzhike.top

Py:   x in arr
来源：http://gou.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://qla.yj20258.top

JS:   arr.includes(x)
来源：http://hay.0kj1m.cn

TS:   arr.includes(x)
来源：http://ufc.zhiwuduotai.top

Java: list.contains(x)
来源：http://ckd.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://thp.bbcook.cn

Ruby: arr.include?(x)
来源：http://vvu.hfpthk.cn

C#:   list.Contains(x)
来源：http://fgg.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://mqh.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kri.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jpy.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rax.pengpengdd.cyou

TS:   [...arr];
来源：http://ymx.hammf.cn

Java: new ArrayList<>(list);
来源：http://txd.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://ktb.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://eff.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://hcc.hfpthk.cn

[D23] reduce 累积计算
来源：http://yqj.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wca.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gni.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipv.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgg.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qtw.snrcjt.cn

Go:   // 手写循环
来源：http://nli.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkk.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qab.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://ejv.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gmg.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cyx.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nyt.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iva.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ykx.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wyi.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hrd.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sfk.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://qhn.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://man.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wci.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ltt.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ogp.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nja.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nxl.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jtl.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bzp.redwolf501.top

[D26] 数组转字符串
来源：http://oxw.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://xhp.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://hga.meibo888.top

JS:   arr.join(", ")
来源：http://oqg.wangdashe.top

TS:   arr.join(", ")
来源：http://vwk.cqqwz.cn

Java: String.join(", ", list)
来源：http://siq.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://xrf.hywenlv.cn

Ruby: arr.join(", ")
来源：http://bkr.nwbrower.top

C#:   string.Join(", ", list)
来源：http://ren.shzxlz.cn

================================================================================
来源：http://occ.mhx1999.top

E. 字符串处理
来源：http://gkj.sufxvd.cn

================================================================================
来源：http://rrb.cdnleiting.top

[E01] 拼接字符串
来源：http://uqg.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xfk.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rbv.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://feu.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yrp.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zct.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jqd.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jta.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://smb.zhixingplan.top

[E02] 重复字符串
来源：http://bsh.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://hyj.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://yoj.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ujv.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://cds.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://dhv.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://srb.gogol.net.cn

Ruby: "ab" * 3
来源：http://ttq.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mut.jiagoushi.top

[E03] 截取子串
来源：http://jdz.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://esb.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://szi.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://azw.wangdashe.top

TS:   s.slice(1, 4)
来源：http://uqm.meibo888.top

Java: s.substring(1, 4)
来源：http://nst.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://krh.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jqv.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://fwd.yj20258888.top

[E04] 查找子串位置
来源：http://awg.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://ghd.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://wyg.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://srt.vehdjk.com

TS:   s.indexOf("x")
来源：http://yqa.havefunace.top

Java: s.indexOf("x")
来源：http://qoc.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://aav.dianchejie.cn

Ruby: s.index("x")
来源：http://rcv.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://oke.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://rex.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xjd.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://erj.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzv.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kjo.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ong.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bus.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://exe.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bxd.vqdsnc.cn

[E06] 替换子串
来源：http://rkl.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tjg.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://skf.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cus.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://vkb.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ntu.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kpc.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fre.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://zdh.tarul.cn

[E07] 按分隔符拆分
来源：http://edp.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lfh.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wet.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uik.aibaodan.cn

TS:   s.split(",")
来源：http://kje.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ibo.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://clz.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://ppl.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wey.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://swf.zhengqikj.top

Py:   ",".join(items)
来源：http://riw.dashuyun.cn

PHP:  implode(",", $items);
来源：http://rov.hnqzz.top

JS:   items.join(",")
来源：http://kju.tanke756.top

TS:   items.join(",")
来源：http://eta.yonumen.top

Java: String.join(",", items)
来源：http://vof.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://pmz.gotoacloud.top

Ruby: items.join(",")
来源：http://nyi.fzhhl.top

C#:   string.Join(",", items)
来源：http://pxa.zdqjudy.top

[E09] 去除所有空白字符
来源：http://zje.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://otp.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qsy.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://pit.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://jdl.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://aoo.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tsb.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://ukq.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://leq.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://usb.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xdg.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cvh.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://uyc.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://bgw.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://iag.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lvj.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tia.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nkd.hnqzz.top

[E11] 反转字符串
来源：http://qvb.fktsv.cn

Py:   s[::-1]
来源：http://xaq.tianlin.xyz

PHP:  strrev($s);
来源：http://gti.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://fvu.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://vtt.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wmn.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://int.tianlin.xyz

Ruby: s.reverse
来源：http://wzj.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://lqu.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://hkt.epnwcf.com

Py:   s.count("a")
来源：http://rwe.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://yar.hammf.cn

JS:   s.split("a").length - 1
来源：http://yyk.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://fqn.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yep.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://dug.dashuyun.cn

Ruby: s.count("a")
来源：http://msy.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://zmn.cashguo.top

[E13] 逐字符遍历
来源：http://ijy.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://vbr.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gxh.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vts.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pke.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ovn.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xby.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vqn.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tjs.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://mrs.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zmo.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvt.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vic.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kxa.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rnq.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drs.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ieu.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xkg.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://xki.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gmg.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rup.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rez.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://adg.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vdf.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sjl.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dic.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pti.zhiwuduotai.top

[E16] 数字千分位
来源：http://xok.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://khu.xziqi.cn


<!-- 参考信息 -->