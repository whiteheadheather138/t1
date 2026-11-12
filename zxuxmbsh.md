代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ksy.jlsjyb.cn

Ruby: arr.sort
来源：http://yvh.gotoacloud.top

C#:   list.Sort();
来源：http://etq.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nuk.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lcc.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gip.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xct.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxe.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mqv.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zxv.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tqx.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cfv.cheryme.top

[D11] 反转数组
来源：http://fam.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rkk.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://jkk.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vwp.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://rga.hysaishi.cn

Java: Collections.reverse(list);
来源：http://kjs.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://pgt.hysaishi.cn

Ruby: arr.reverse
来源：http://eth.shangyingyoupin.top

C#:   list.Reverse();
来源：http://gtj.ivvv.top

[D12] 查找元素下标
来源：http://dbd.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://dro.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rbq.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zro.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ygo.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hcu.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://lps.tarul.cn

Ruby: arr.index(x)
来源：http://vzs.meibo888.top

C#:   list.IndexOf(x);
来源：http://aij.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://wuw.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uwi.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nsk.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://oma.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://aof.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mqs.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wsu.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://zpg.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://obx.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://hvy.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dat.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dpn.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://bcf.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://acl.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mej.nwbrower.top

Go:   // 手写循环
来源：http://suu.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lwr.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dei.smart0.xyz

[D15] 去重
来源：http://rej.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vmz.pycfn.com

PHP:  array_unique($arr);
来源：http://edp.mhx1999.top

JS:   [...new Set(arr)]
来源：http://zpf.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://clx.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cvr.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://tfx.chenjidiqi.icu

Ruby: arr.uniq
来源：http://sxs.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://hvv.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://sdu.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xnp.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xht.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpe.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ere.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ygp.svipenyu.cn

Go:   // 手写循环累加
来源：http://sdf.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mdz.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://rdk.zhengqikj.top

[D17] 最大值与最小值
来源：http://egr.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://rjp.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://kou.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tty.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://ajz.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cbv.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nkf.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://uku.sweek.top

C#:   list.Max();  list.Min()
来源：http://yel.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://irz.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mjt.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://cpr.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jdf.xziqi.cn

TS:   nested.flat();
来源：http://fpw.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvq.zhongyouzk.top

Go:   // 手写双层循环
来源：http://ucu.vehdjk.com

Ruby: nested.flatten
来源：http://vcp.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vky.52xcode.cn

[D19] 按字段分组
来源：http://hye.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xke.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://izd.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wlr.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pke.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibx.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://klp.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://suq.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nyn.yongpay.top

[D20] 统计每个元素出现次数
来源：http://wws.epnwcf.com

Py:   Counter(arr)
来源：http://jvc.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://ife.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgx.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://idx.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ios.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://kda.hysaishi.cn

Ruby: arr.tally
来源：http://hea.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fnm.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://cpn.quarkkingdee.top

Py:   x in arr
来源：http://lul.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://pwh.xylfe.cn

JS:   arr.includes(x)
来源：http://ojg.jianghu66.top

TS:   arr.includes(x)
来源：http://bcm.hfpthk.cn

Java: list.contains(x)
来源：http://acm.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://sjh.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://kzk.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://fhb.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://pvm.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yee.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lrn.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vvu.quarkkingdee.top

TS:   [...arr];
来源：http://tnh.tian-w.cn

Java: new ArrayList<>(list);
来源：http://sbd.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://mvb.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://ckt.gotoacloud.top

C#:   new List<int>(list);
来源：http://uzp.yongpay.top

[D23] reduce 累积计算
来源：http://qce.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cqi.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ris.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bww.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpc.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://cmi.jyoumei.cn

Go:   // 手写循环
来源：http://kxq.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fit.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://odz.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://ggu.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ozr.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hye.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hmt.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jjn.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://orv.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xdl.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dmd.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kwz.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://oqx.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zyt.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://igh.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qoh.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://msz.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bhd.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qbt.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tkp.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwz.cheryme.top

[D26] 数组转字符串
来源：http://eal.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://cez.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://owz.svipenyu.cn

JS:   arr.join(", ")
来源：http://kjv.cucudq.cn

TS:   arr.join(", ")
来源：http://jqg.hcnkem.com

Java: String.join(", ", list)
来源：http://sws.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://azr.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://cad.wangdashe.top

C#:   string.Join(", ", list)
来源：http://msv.vehdjk.com

================================================================================
来源：http://pzi.bjfxy.top

E. 字符串处理
来源：http://rti.shanyushiyangkeji.top

================================================================================
来源：http://sre.ydjk.org.cn

[E01] 拼接字符串
来源：http://uqy.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nht.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hpt.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ufw.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfv.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sxe.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oqb.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oij.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wug.fanxiaobao.xyz

[E02] 重复字符串
来源：http://jwd.ydzc1.top

Py:   "ab" * 3
来源：http://pgb.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://guo.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://jtc.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://zkf.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://ieq.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://ssm.zhengqikj.top

Ruby: "ab" * 3
来源：http://dfc.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ckk.chenlongwang.top

[E03] 截取子串
来源：http://pvk.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnw.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rlj.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dkt.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://vjw.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://niw.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qto.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://dxq.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://fmo.jiagoushi.top

[E04] 查找子串位置
来源：http://pja.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://rwy.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://juq.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pcc.havefunace.top

TS:   s.indexOf("x")
来源：http://muw.hnqzz.top

Java: s.indexOf("x")
来源：http://tnj.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://cbk.zhijiandao.cn

Ruby: s.index("x")
来源：http://hpt.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://rrv.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uob.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oer.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ypj.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ugt.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ujy.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxi.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dis.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nze.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kep.yj20258888.top

[E06] 替换子串
来源：http://zgd.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://psk.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://ksf.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dze.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://gsw.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqn.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tig.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eqj.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://ydw.fengsongda.top

[E07] 按分隔符拆分
来源：http://okf.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nej.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://opp.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwn.gogol.net.cn

TS:   s.split(",")
来源：http://asl.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xyh.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bvw.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://zsd.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ter.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://zgu.sufxvd.cn

Py:   ",".join(items)
来源：http://zax.yonumen.top

PHP:  implode(",", $items);
来源：http://gtx.yfazqb.com

JS:   items.join(",")
来源：http://egt.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://igd.xziqi.cn

Java: String.join(",", items)
来源：http://ygz.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://oae.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://zvf.bbcook.cn

C#:   string.Join(",", items)
来源：http://snm.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://owl.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lmm.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bvg.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://cxi.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://nqw.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://hfz.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yqq.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://suq.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qjc.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://ngq.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zoo.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pbi.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://fsl.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://fuv.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://qew.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://fvz.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zno.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aoi.fktsv.cn

[E11] 反转字符串
来源：http://dhr.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://zoq.jinqigufen.top

PHP:  strrev($s);
来源：http://rnb.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://xpj.tarul.cn

TS:   [...s].reverse().join("")
来源：http://dci.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rox.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dvv.mhx1999.top

Ruby: s.reverse
来源：http://mgh.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://zcq.tanke756.top

[E12] 统计某字符出现次数
来源：http://clm.xuetiantiany.cn

Py:   s.count("a")
来源：http://mgg.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://fvc.aizwys.cn

JS:   s.split("a").length - 1
来源：http://cvn.ydzc1.top

TS:   s.split("a").length - 1
来源：http://dds.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hhq.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://kiy.jinqigufen.top

Ruby: s.count("a")
来源：http://upz.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://mcn.haohaochexian.top

[E13] 逐字符遍历
来源：http://evm.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://pda.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vdb.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://emi.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nvi.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mpe.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xom.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gig.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ewr.iojbl.cn

[E14] URL 编码与 Base64
来源：http://svh.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jfa.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://leq.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zuw.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xpu.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nzv.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ecz.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kan.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://krd.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://dyi.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aon.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dgm.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://khj.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bgy.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vnr.yonumen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zcg.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wyy.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oml.tanke756.top

[E16] 数字千分位
来源：http://tbd.daria6918.cn

Py:   f"{1234567:,}"
来源：http://dsj.havefunace.top

PHP:  number_format(1234567);
来源：http://pdi.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zdh.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bxx.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jkj.andypj.xyz


<!-- 参考信息 -->