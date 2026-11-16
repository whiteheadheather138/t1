代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cns.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://loc.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://frx.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oaz.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pvh.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pwe.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nef.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://myl.bjfxy.top

[D11] 反转数组
来源：http://oxy.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://exe.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://aoi.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gdn.sufxvd.cn

TS:   [...arr].reverse();
来源：http://cyp.yj20258.top

Java: Collections.reverse(list);
来源：http://iys.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://qgr.jiagoushi.top

Ruby: arr.reverse
来源：http://dvh.gogol.net.cn

C#:   list.Reverse();
来源：http://dfu.yuxming.cn

[D12] 查找元素下标
来源：http://eqa.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://jiv.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eog.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gik.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jjv.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vgs.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://lfq.hywenlv.cn

Ruby: arr.index(x)
来源：http://aig.daxiang520.top

C#:   list.IndexOf(x);
来源：http://vuz.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://qjy.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hqm.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://efa.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://mmd.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://axs.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zji.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gtj.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://xlt.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://myt.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://gpg.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ftl.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lrp.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://lkx.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://hvd.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kse.iojbl.cn

Go:   // 手写循环
来源：http://fhs.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gsp.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://qja.ywan-chungtsiang.top

[D15] 去重
来源：http://jsi.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kae.jqgfzy.top

PHP:  array_unique($arr);
来源：http://dln.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://qki.xinyue.icu

TS:   [...new Set(arr)]
来源：http://nop.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://drq.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://btn.sysykeji.top

Ruby: arr.uniq
来源：http://phm.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://fjv.hammf.cn

[D16] 求和与平均值
来源：http://fbp.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gxv.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kqb.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://odh.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qvy.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sqk.andypj.xyz

Go:   // 手写循环累加
来源：http://znp.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pin.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://hqh.ctjpmb.com

[D17] 最大值与最小值
来源：http://mam.uphjek.com

Py:   max(arr);  min(arr)
来源：http://eis.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://jbp.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wqy.xuanzx.com

TS:   Math.max(...arr);
来源：http://wua.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jxq.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eef.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://cgy.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://lab.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://xwh.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qqn.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://afz.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fmd.dashuyun.cn

TS:   nested.flat();
来源：http://nzs.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nsi.zycfv.cn

Go:   // 手写双层循环
来源：http://lda.uphjek.com

Ruby: nested.flatten
来源：http://uzk.jinqigufen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hbl.haohaochexian.top

[D19] 按字段分组
来源：http://hfx.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://koo.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gav.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dhu.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ceo.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gnc.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://bid.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vkx.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ozo.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://hfm.xuanzx.com

Py:   Counter(arr)
来源：http://wgy.vehdjk.com

PHP:  array_count_values($arr);
来源：http://bpj.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mhm.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pse.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fkm.andypj.xyz

Go:   // 手写 map[T]int
来源：http://ojt.jinqigfzy.top

Ruby: arr.tally
来源：http://tgv.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zur.hcnkem.com

[D21] 判断是否包含某元素
来源：http://mrk.c1oappe.top

Py:   x in arr
来源：http://tot.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://kmv.andypj.xyz

JS:   arr.includes(x)
来源：http://wof.yvedp.cn

TS:   arr.includes(x)
来源：http://ukj.ydzc1.top

Java: list.contains(x)
来源：http://gcq.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://mze.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://tox.yongpay.top

C#:   list.Contains(x)
来源：http://vnk.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://srk.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iat.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpb.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tfj.yvedp.cn

TS:   [...arr];
来源：http://bye.zycfv.cn

Java: new ArrayList<>(list);
来源：http://uvt.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://dvg.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://orf.bbcook.cn

C#:   new List<int>(list);
来源：http://rhb.zhoulong.xyz

[D23] reduce 累积计算
来源：http://icj.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lte.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ick.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vkx.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://juh.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hxx.yanxiufei.cn

Go:   // 手写循环
来源：http://vly.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dui.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yzr.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://ofc.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ubr.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://waw.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfu.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://byy.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gzb.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fve.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sls.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wwg.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://ubs.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kmp.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yaw.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mrf.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hye.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ury.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvt.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zuv.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pyi.zhiwuduotai.top

[D26] 数组转字符串
来源：http://wxb.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://hkz.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://vhz.hfpthk.cn

JS:   arr.join(", ")
来源：http://bok.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://fea.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://cim.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://sxl.yonumen.top

Ruby: arr.join(", ")
来源：http://euh.yvedp.cn

C#:   string.Join(", ", list)
来源：http://xmf.yuanzhike.top

================================================================================
来源：http://nat.kuanghao11.cn

E. 字符串处理
来源：http://cvp.yvedp.cn

================================================================================
来源：http://nwd.yuxming.cn

[E01] 拼接字符串
来源：http://qfa.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dna.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ewh.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qzr.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ayy.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wet.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uvu.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zdf.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fes.yvedp.cn

[E02] 重复字符串
来源：http://sfl.dianchejie.cn

Py:   "ab" * 3
来源：http://rwh.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://ixr.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://kos.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://hax.gotoacloud.top

Java: "ab".repeat(3)
来源：http://mzs.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://itv.mhx1999.top

Ruby: "ab" * 3
来源：http://sbp.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jeh.yuxming.cn

[E03] 截取子串
来源：http://jci.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tcw.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dfj.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csv.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://loh.hammf.cn

Java: s.substring(1, 4)
来源：http://gwc.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ewk.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://rxb.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://uhr.tian-w.cn

[E04] 查找子串位置
来源：http://svo.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://akm.yvedp.cn

PHP:  strpos($s, "x");
来源：http://der.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xyy.hcnkem.com

TS:   s.indexOf("x")
来源：http://jsz.tanke756.top

Java: s.indexOf("x")
来源：http://yur.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://sno.zdbjq.cn

Ruby: s.index("x")
来源：http://jsn.xuanzx.com

C#:   s.IndexOf("x")
来源：http://qki.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://plc.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://acu.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://njk.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akp.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://jmx.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://boh.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fsm.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jdx.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pxk.xziqi.cn

[E06] 替换子串
来源：http://ghi.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://llx.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://vra.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yqe.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://pmt.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://unl.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iyt.ivvv.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nwe.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://yqf.yangfankeji.com

[E07] 按分隔符拆分
来源：http://ayq.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zlq.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dxg.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oug.xylfe.cn

TS:   s.split(",")
来源：http://wyy.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://goh.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yns.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://spc.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ugq.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://ucq.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://dbx.cheryme.top

PHP:  implode(",", $items);
来源：http://krb.redwolf501.top

JS:   items.join(",")
来源：http://kqw.jinqigufen.top

TS:   items.join(",")
来源：http://rta.zycfv.cn

Java: String.join(",", items)
来源：http://frn.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://pyg.fehbvm.com

Ruby: items.join(",")
来源：http://obv.jianghu66.top

C#:   string.Join(",", items)
来源：http://rhb.0kj1m.cn

[E09] 去除所有空白字符
来源：http://abf.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mam.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fxa.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://irn.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://caw.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://gui.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://zjy.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://smy.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ujr.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://zbb.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://abe.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vps.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://qzr.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://aon.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://pgo.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bpf.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zaj.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mlo.dashuyun.cn

[E11] 反转字符串
来源：http://fnj.fehbvm.com

Py:   s[::-1]
来源：http://whv.yanxiufei.cn

PHP:  strrev($s);
来源：http://vgc.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://pzq.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://prk.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dbe.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qlg.zdbjq.cn

Ruby: s.reverse
来源：http://yiv.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zfv.fktsv.cn

[E12] 统计某字符出现次数
来源：http://ine.pengpengdd.cyou

Py:   s.count("a")
来源：http://hok.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://cjv.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://cjd.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://lgs.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lkj.tarul.cn

Go:   strings.Count(s, "a")
来源：http://ixj.9152youxi.cn

Ruby: s.count("a")
来源：http://gbb.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://hog.sweek.top

[E13] 逐字符遍历
来源：http://ebj.yj202588.top

Py:   for ch in s: print(ch)
来源：http://tlm.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vem.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oco.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tcp.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ezl.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ueu.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jgb.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uod.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://yiz.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vnr.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://obg.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hoe.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wdt.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qbi.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tjq.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yib.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zkp.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://vwu.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://koz.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lpp.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lxg.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rnl.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://okj.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nja.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://swm.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zgq.xziqi.cn

[E16] 数字千分位
来源：http://keo.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://nks.jinqigufen.top

PHP:  number_format(1234567);
来源：http://uze.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://qit.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cwk.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mpe.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jtd.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgs.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://fov.iojbl.cn

[E17] 首字母大写
来源：http://lii.zhoulong.xyz


<!-- 参考信息 -->