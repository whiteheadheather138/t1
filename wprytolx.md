代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wlq.9152youxi.cn

Ruby: arr.sort
来源：http://bni.zycfv.cn

C#:   list.Sort();
来源：http://kvo.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rxi.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbm.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xsv.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvf.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iie.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cig.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gsq.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://exw.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://axv.haohaochexian.top

[D11] 反转数组
来源：http://ffp.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://fga.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://thi.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hkp.bjfxy.top

TS:   [...arr].reverse();
来源：http://jpm.zhengqikj.top

Java: Collections.reverse(list);
来源：http://cdt.tarul.cn

Go:   slices.Reverse(arr)
来源：http://utf.iojbl.cn

Ruby: arr.reverse
来源：http://jie.xinyue.icu

C#:   list.Reverse();
来源：http://kyw.dashuyun.cn

[D12] 查找元素下标
来源：http://kjx.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://rch.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://abj.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zxt.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bol.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cjs.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://tvc.ctjpmb.com

Ruby: arr.index(x)
来源：http://brj.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://quu.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://kgv.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://skq.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zfe.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://aik.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://erg.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hwy.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vov.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://uwo.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ehb.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://hpq.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dmx.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vwe.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://uxk.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://hof.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzv.yangfankeji.com

Go:   // 手写循环
来源：http://rza.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://xum.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ohl.jinqigufen.top

[D15] 去重
来源：http://oyx.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eda.sxryk.cn

PHP:  array_unique($arr);
来源：http://bvg.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://rdv.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://mfa.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgq.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mlu.hesvh.cn

Ruby: arr.uniq
来源：http://whb.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://xeo.redwolf501.top

[D16] 求和与平均值
来源：http://qwf.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cjm.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zzs.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdy.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://awr.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ylh.ydjk.org.cn

Go:   // 手写循环累加
来源：http://cct.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://srg.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://ypw.dashuyun.cn

[D17] 最大值与最小值
来源：http://tcg.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://yvv.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://eto.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hzz.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://awe.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lev.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ywe.yj202588.top

Ruby: arr.max;  arr.min
来源：http://deq.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://uqa.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://gzq.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tnb.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://hwa.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jpy.hfpthk.cn

TS:   nested.flat();
来源：http://nas.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zen.aibaodan.cn

Go:   // 手写双层循环
来源：http://lma.0kj1m.cn

Ruby: nested.flatten
来源：http://gxm.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgd.pycfn.com

[D19] 按字段分组
来源：http://fnx.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://alq.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jta.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rbp.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://izn.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bmp.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://jag.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bnk.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://neu.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://kbz.ctjpmb.com

Py:   Counter(arr)
来源：http://sjw.epnwcf.com

PHP:  array_count_values($arr);
来源：http://pvl.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgc.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vjg.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vcj.sxryk.cn

Go:   // 手写 map[T]int
来源：http://dcv.chenjidiqi.icu

Ruby: arr.tally
来源：http://qhx.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zlo.xziqi.cn

[D21] 判断是否包含某元素
来源：http://wse.bbcook.cn

Py:   x in arr
来源：http://pnb.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://ibj.bbcook.cn

JS:   arr.includes(x)
来源：http://cfm.zhoulong.xyz

TS:   arr.includes(x)
来源：http://duw.pycfn.com

Java: list.contains(x)
来源：http://ign.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://euy.snrcjt.cn

Ruby: arr.include?(x)
来源：http://hkp.gotoacloud.top

C#:   list.Contains(x)
来源：http://pjl.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://etz.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pmz.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uiu.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cuo.redwolf501.top

TS:   [...arr];
来源：http://hlo.havefunace.top

Java: new ArrayList<>(list);
来源：http://efi.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mdq.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://jpo.zdbjq.cn

C#:   new List<int>(list);
来源：http://ugi.ppjwa.cn

[D23] reduce 累积计算
来源：http://ilu.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oiv.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lhz.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zwk.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shn.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bhm.316326.xyz

Go:   // 手写循环
来源：http://vhf.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hap.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pxv.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://jep.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xuy.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://msq.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cip.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bxg.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pqe.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fnl.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://inn.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lde.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://qpk.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ozr.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fdj.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngb.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xor.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kmh.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmp.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hod.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqp.dashuyun.cn

[D26] 数组转字符串
来源：http://foz.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://hwh.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://swd.pycfn.com

JS:   arr.join(", ")
来源：http://lhy.hywenlv.cn

TS:   arr.join(", ")
来源：http://aso.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://zmg.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://jfc.nanxinkj.top

Ruby: arr.join(", ")
来源：http://ujv.uphjek.com

C#:   string.Join(", ", list)
来源：http://oze.gaohongyu789.top

================================================================================
来源：http://uip.zhijiandao.cn

E. 字符串处理
来源：http://ejl.nanxinkj.top

================================================================================
来源：http://zvn.feifeiyinyue.top

[E01] 拼接字符串
来源：http://ffa.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ctt.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ojy.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yqn.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpj.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ggt.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://agn.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hvk.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mpm.hammf.cn

[E02] 重复字符串
来源：http://ikh.tianlin.xyz

Py:   "ab" * 3
来源：http://xwg.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://bzu.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://wik.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://otz.gogol.net.cn

Java: "ab".repeat(3)
来源：http://stz.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://sze.hnqzz.top

Ruby: "ab" * 3
来源：http://cwt.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://imu.guannengcc.top

[E03] 截取子串
来源：http://mcz.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xep.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xnj.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qdb.yonumen.top

TS:   s.slice(1, 4)
来源：http://bqn.epnwcf.com

Java: s.substring(1, 4)
来源：http://cue.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://whg.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://iky.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://hqz.zdbjq.cn

[E04] 查找子串位置
来源：http://ftr.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://cmd.yfazqb.com

PHP:  strpos($s, "x");
来源：http://sgi.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://egd.yuanzhike.top

TS:   s.indexOf("x")
来源：http://cld.fengsongda.top

Java: s.indexOf("x")
来源：http://qwa.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://hrh.snrcjt.cn

Ruby: s.index("x")
来源：http://dyw.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://pjr.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rdn.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mwd.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zal.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtw.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vyv.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mou.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://roh.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dfz.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thi.fktsv.cn

[E06] 替换子串
来源：http://mvs.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kks.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://qzy.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyy.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://vbl.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sru.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pog.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kum.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://wgc.dianchejie.cn

[E07] 按分隔符拆分
来源：http://tiq.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jyr.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wds.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hcr.yueranfly.top

TS:   s.split(",")
来源：http://xou.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://cdv.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kxx.hammf.cn

Ruby: s.split(",");  s.split
来源：http://vjn.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nzz.c1oappe.top

[E08] 数组按分隔符合并
来源：http://vsl.yongpay.top

Py:   ",".join(items)
来源：http://ymk.gogol.net.cn

PHP:  implode(",", $items);
来源：http://roe.chenjidiqi.icu

JS:   items.join(",")
来源：http://rpq.svipenyu.cn

TS:   items.join(",")
来源：http://dgj.epnwcf.com

Java: String.join(",", items)
来源：http://kpo.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://ubr.kuanghao11.cn

Ruby: items.join(",")
来源：http://iaf.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://dfi.guannengcc.top

[E09] 去除所有空白字符
来源：http://ypf.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://voy.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qcf.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://gzt.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://spx.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://vyc.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kfg.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xla.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gst.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://sup.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qwf.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://grq.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://viv.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://zph.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://gad.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ofz.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://geg.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wrq.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://zis.gzhubu.top

Py:   s[::-1]
来源：http://dvq.yanxiufei.cn

PHP:  strrev($s);
来源：http://coh.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://bbm.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://eos.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://efw.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://azs.guannengcc.top

Ruby: s.reverse
来源：http://koj.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://rle.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://hlg.xziqi.cn

Py:   s.count("a")
来源：http://rjp.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://zff.mhx1999.top

JS:   s.split("a").length - 1
来源：http://qvs.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://atc.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nyc.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://jjq.wangshuangyany.cn

Ruby: s.count("a")
来源：http://wvf.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://kyu.wangdashe.top

[E13] 逐字符遍历
来源：http://zhf.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://hgc.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yay.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://roe.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gvx.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gla.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jec.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://voa.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hbj.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://rvo.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rlz.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zos.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tlg.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://etj.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hnl.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tzn.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tsa.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eft.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://ulu.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://svb.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nab.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gcg.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://owh.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zum.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kcr.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tui.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hxf.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://tou.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://wde.haohaochexian.top

PHP:  number_format(1234567);
来源：http://fff.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://epq.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xgk.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cxi.sxryk.cn


<!-- 参考信息 -->