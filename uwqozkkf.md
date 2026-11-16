代发 wailian999

TS:   arr.slice(1, 4);
来源：http://fgz.epnwcf.com

Java: list.subList(1, 4);
来源：http://bew.havefunace.top

Go:   arr[1:4]
来源：http://nfu.zhengqikj.top

Ruby: arr[1, 3]
来源：http://kkv.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://hdj.bjfxy.top

[D08] 合并两个数组
来源：http://xhu.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://zzb.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://nuz.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zwr.hnxiangtu.top

TS:   [...a, ...b];
来源：http://bnp.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mrx.sjlbkw.cn

Go:   append(a, b...)
来源：http://cdc.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://iyz.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://eqv.gaohongyu789.top

[D09] 排序（升序）
来源：http://ecb.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://dit.9152youxi.cn

PHP:  sort($arr);
来源：http://euj.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gvx.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://agp.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kzg.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blu.snrcjt.cn

Ruby: arr.sort
来源：http://uya.shanyushiyangtech.top

C#:   list.Sort();
来源：http://ydz.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vpe.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://din.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hta.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://msf.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ant.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vdb.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://elb.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vky.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ecr.cdnleiting.top

[D11] 反转数组
来源：http://ixk.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://quk.yonumen.top

PHP:  array_reverse($arr);
来源：http://uli.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cfw.nanxinkj.top

TS:   [...arr].reverse();
来源：http://sdw.jyoumei.cn

Java: Collections.reverse(list);
来源：http://iqt.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://lab.9152youxi.cn

Ruby: arr.reverse
来源：http://ngc.chenlongwang.top

C#:   list.Reverse();
来源：http://oqs.nanxuanxn.top

[D12] 查找元素下标
来源：http://ffr.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://thg.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ekv.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcl.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fwa.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhl.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://yvg.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://upj.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://efd.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://kbw.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uou.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ood.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://xfe.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://trt.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://urt.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://upt.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://vua.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://laj.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://jyv.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bcc.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xim.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://lcm.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://xka.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eio.yj20258888.top

Go:   // 手写循环
来源：http://rqy.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://ndc.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uje.ywan-chungtsiang.top

[D15] 去重
来源：http://tjt.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qjt.gogol.net.cn

PHP:  array_unique($arr);
来源：http://xkz.uphjek.com

JS:   [...new Set(arr)]
来源：http://wps.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://kim.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ztj.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fbs.tianlin.xyz

Ruby: arr.uniq
来源：http://xjb.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://bqs.yj202588.top

[D16] 求和与平均值
来源：http://yhp.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rqj.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iwl.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgt.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ato.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sjt.xziqi.cn

Go:   // 手写循环累加
来源：http://mfw.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqx.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://azp.havefunace.top

[D17] 最大值与最小值
来源：http://fxo.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://afg.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://xdz.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ckj.yueranfly.top

TS:   Math.max(...arr);
来源：http://sle.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mfg.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgo.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://ukh.cashguo.top

C#:   list.Max();  list.Min()
来源：http://zmq.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://rwi.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pwh.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://kck.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sis.yangfankeji.com

TS:   nested.flat();
来源：http://rjz.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://luj.tanke756.top

Go:   // 手写双层循环
来源：http://fwv.yvedp.cn

Ruby: nested.flatten
来源：http://vbp.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rst.jiagoushi.top

[D19] 按字段分组
来源：http://jtk.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://axs.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gcl.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dor.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zkm.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lvj.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://bor.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xbe.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://clp.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://too.bjfxy.top

Py:   Counter(arr)
来源：http://zaa.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://ysj.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqg.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zar.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jus.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://frd.aibaodan.cn

Ruby: arr.tally
来源：http://une.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iqf.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://yee.sjlbkw.cn

Py:   x in arr
来源：http://xpk.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://arn.nwbrower.top

JS:   arr.includes(x)
来源：http://zlz.jiagoushi.top

TS:   arr.includes(x)
来源：http://cty.c1oappe.top

Java: list.contains(x)
来源：http://raj.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://ngs.epnwcf.com

Ruby: arr.include?(x)
来源：http://uns.zdbjq.cn

C#:   list.Contains(x)
来源：http://ete.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://mzg.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oen.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eyi.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pvp.pycfn.com

TS:   [...arr];
来源：http://nif.uphjek.com

Java: new ArrayList<>(list);
来源：http://gqw.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://syj.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://jof.ivvv.top

C#:   new List<int>(list);
来源：http://beb.jinqigfzy.top

[D23] reduce 累积计算
来源：http://gxc.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yxm.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yyb.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nta.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwi.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://prb.snrcjt.cn

Go:   // 手写循环
来源：http://ejc.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pde.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zsg.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://gdb.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://and.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pxy.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xve.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ojf.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xpy.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qfi.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mbu.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kzx.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://bnp.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://goh.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lxs.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cry.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tet.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgy.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nco.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nsy.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rjm.hammf.cn

[D26] 数组转字符串
来源：http://swn.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://vou.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://obo.xylfe.cn

JS:   arr.join(", ")
来源：http://krv.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://ueo.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://jye.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://tds.jinqigufen.top

Ruby: arr.join(", ")
来源：http://cuc.mhx1999.top

C#:   string.Join(", ", list)
来源：http://kcr.mhx1999.top

================================================================================
来源：http://xxd.hfpthk.cn

E. 字符串处理
来源：http://knq.cqqwz.cn

================================================================================
来源：http://tur.ctjpmb.com

[E01] 拼接字符串
来源：http://kbh.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yvf.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qjg.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lli.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://chv.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ywh.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hgn.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://srh.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bic.gotoacloud.top

[E02] 重复字符串
来源：http://oiy.xylfe.cn

Py:   "ab" * 3
来源：http://xsd.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://ezs.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://fda.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://sag.iojbl.cn

Java: "ab".repeat(3)
来源：http://luw.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://zco.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://rza.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://noh.dianchejie.cn

[E03] 截取子串
来源：http://svn.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxh.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mfp.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nrd.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://csi.yj20258.top

Java: s.substring(1, 4)
来源：http://gjt.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dps.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://ruu.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://ifj.yfazqb.com

[E04] 查找子串位置
来源：http://vld.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://wkg.smart0.xyz

PHP:  strpos($s, "x");
来源：http://zfj.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cyc.dashuyun.cn

TS:   s.indexOf("x")
来源：http://qeg.fehbvm.com

Java: s.indexOf("x")
来源：http://zta.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://imj.cucudq.cn

Ruby: s.index("x")
来源：http://vew.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://fsx.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xee.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kaq.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uim.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lmz.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://blx.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glc.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mil.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nku.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rlc.daxiang520.top

[E06] 替换子串
来源：http://ltt.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zgv.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ufk.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xtq.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://iwn.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llu.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://onf.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ewl.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://tjo.jqgfzy.top

[E07] 按分隔符拆分
来源：http://hha.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwe.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aam.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://quw.hysaishi.cn

TS:   s.split(",")
来源：http://uhp.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://wfs.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dkp.yonumen.top

Ruby: s.split(",");  s.split
来源：http://ame.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mnc.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://gmf.xuetiantiany.cn

Py:   ",".join(items)
来源：http://uxm.ydzc1.top

PHP:  implode(",", $items);
来源：http://euo.sweek.top

JS:   items.join(",")
来源：http://ftu.sxryk.cn

TS:   items.join(",")
来源：http://mhr.yj20258888.top

Java: String.join(",", items)
来源：http://uaz.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://rdj.ivvv.top

Ruby: items.join(",")
来源：http://jbv.gotoacloud.top

C#:   string.Join(",", items)
来源：http://kcs.bjfxy.top

[E09] 去除所有空白字符
来源：http://vrk.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bra.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xtx.0kj1m.cn

JS:   s.replace(/\s+/g, "")
来源：http://rmc.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://fui.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://bsg.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gmc.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://djc.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qaf.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://oir.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wty.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iap.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://blx.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://ely.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://veb.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://akw.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zov.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aih.quarkkingdee.top

[E11] 反转字符串
来源：http://fgg.sjlbkw.cn

Py:   s[::-1]
来源：http://anw.hesvh.cn

PHP:  strrev($s);
来源：http://zcq.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://rmg.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://vxn.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qyz.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zao.316326.xyz

Ruby: s.reverse
来源：http://zmf.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://sav.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://fyu.vqdsnc.cn

Py:   s.count("a")
来源：http://nkg.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://lkg.redwolf501.top

JS:   s.split("a").length - 1
来源：http://qfk.bbcook.cn

TS:   s.split("a").length - 1
来源：http://lkr.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bzm.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://vhz.hysaishi.cn

Ruby: s.count("a")
来源：http://qgr.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://gfd.guowangkeji.top

[E13] 逐字符遍历
来源：http://khj.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://eyq.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tnx.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mrr.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://odu.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfl.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://icp.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uev.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cci.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://zms.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mvq.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zsy.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mvl.yanxiufei.cn


<!-- 参考信息 -->