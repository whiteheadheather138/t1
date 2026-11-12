代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yxo.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mey.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ing.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ura.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ker.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ulw.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://npg.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uiw.aibaodan.cn

[D11] 反转数组
来源：http://bxz.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://nkr.tanke756.top

PHP:  array_reverse($arr);
来源：http://yiw.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://auo.wangdashe.top

TS:   [...arr].reverse();
来源：http://hiv.shzxlz.cn

Java: Collections.reverse(list);
来源：http://osl.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://wzn.zhijiandao.cn

Ruby: arr.reverse
来源：http://xqk.chenjidiqi.icu

C#:   list.Reverse();
来源：http://ccb.fengsongda.top

[D12] 查找元素下标
来源：http://eup.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://wgh.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://srv.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ebb.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdn.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gyx.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://wyg.hnxiangtu.top

Ruby: arr.index(x)
来源：http://mhv.mhx1999.top

C#:   list.IndexOf(x);
来源：http://jwd.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://wql.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hll.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tkw.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://zrt.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://kxz.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcc.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cww.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bpm.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oua.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://ufo.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oue.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wsh.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://tra.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://wah.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ylf.aibaodan.cn

Go:   // 手写循环
来源：http://fdz.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://epl.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://piy.ybcxt.top

[D15] 去重
来源：http://war.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rcs.hysaishi.cn

PHP:  array_unique($arr);
来源：http://wwt.52xcode.cn

JS:   [...new Set(arr)]
来源：http://cgu.uphjek.com

TS:   [...new Set(arr)]
来源：http://pkf.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cyt.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://ddv.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://cmy.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://fej.sufxvd.cn

[D16] 求和与平均值
来源：http://vxw.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jho.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dak.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gim.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dku.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tkx.kuanghao11.cn

Go:   // 手写循环累加
来源：http://dks.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fdu.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://hvi.cashguo.top

[D17] 最大值与最小值
来源：http://ghw.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://vgv.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://wvo.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tab.aibaodan.cn

TS:   Math.max(...arr);
来源：http://tqr.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://qgo.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hhl.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://fdj.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://zih.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://awg.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ghs.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://ucq.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bnz.havefunace.top

TS:   nested.flat();
来源：http://kpe.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jhi.nanxuanxn.top

Go:   // 手写双层循环
来源：http://kry.yfazqb.com

Ruby: nested.flatten
来源：http://gre.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://djb.guannengcc.top

[D19] 按字段分组
来源：http://gka.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hiy.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pnb.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ntn.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iqc.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zif.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://nxf.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://chq.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ohg.uphjek.com

[D20] 统计每个元素出现次数
来源：http://egd.ydzc1.top

Py:   Counter(arr)
来源：http://fku.uphjek.com

PHP:  array_count_values($arr);
来源：http://paq.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bea.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kub.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lef.yj202588.top

Go:   // 手写 map[T]int
来源：http://psu.fzhhl.top

Ruby: arr.tally
来源：http://vmb.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xdq.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://sbe.chenzaomai.com

Py:   x in arr
来源：http://gln.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://llo.gaohongyu789.top

JS:   arr.includes(x)
来源：http://xic.yonumen.top

TS:   arr.includes(x)
来源：http://ljr.cheryme.top

Java: list.contains(x)
来源：http://cee.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://vko.meibo888.top

Ruby: arr.include?(x)
来源：http://vll.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://nbn.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://xkz.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vbe.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gus.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://siy.fktsv.cn

TS:   [...arr];
来源：http://bik.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://dvk.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://knf.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://snw.ivvv.top

C#:   new List<int>(list);
来源：http://yak.yuanzhike.top

[D23] reduce 累积计算
来源：http://fcc.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bzd.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rpt.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yoe.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipe.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nyi.epnwcf.com

Go:   // 手写循环
来源：http://yci.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uks.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://puv.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://tct.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xjc.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obi.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xll.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lly.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgl.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ran.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hgg.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hqe.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://izk.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hed.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zff.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gaa.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bio.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sxb.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vat.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fja.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hzm.shzxlz.cn

[D26] 数组转字符串
来源：http://yqu.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://xwh.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://cce.fengsongda.top

JS:   arr.join(", ")
来源：http://vzr.52xcode.cn

TS:   arr.join(", ")
来源：http://rnp.cqqwz.cn

Java: String.join(", ", list)
来源：http://gwn.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://qpa.gzhubu.top

Ruby: arr.join(", ")
来源：http://tmr.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://ikw.c1oappe.top

================================================================================
来源：http://tpj.cashguo.top

E. 字符串处理
来源：http://nmw.wangdashe.top

================================================================================
来源：http://bjo.yvedp.cn

[E01] 拼接字符串
来源：http://yoh.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qev.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wxi.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sui.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwd.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gtz.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mhv.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tvn.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fub.wangdashe.top

[E02] 重复字符串
来源：http://wed.jqgufenzy.top

Py:   "ab" * 3
来源：http://kjc.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://adj.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://vry.andypj.xyz

TS:   "ab".repeat(3)
来源：http://pme.yuanzhike.top

Java: "ab".repeat(3)
来源：http://ybb.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://vks.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://nxs.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://shf.fktsv.cn

[E03] 截取子串
来源：http://zee.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gxr.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbh.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lkz.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://arx.mhx1999.top

Java: s.substring(1, 4)
来源：http://txa.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ffy.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pms.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://zag.ctjpmb.com

[E04] 查找子串位置
来源：http://ijw.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://kdz.fengsongda.top

PHP:  strpos($s, "x");
来源：http://hid.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rip.hywenlv.cn

TS:   s.indexOf("x")
来源：http://gbz.yuxming.cn

Java: s.indexOf("x")
来源：http://oht.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://lwv.zhongyouzk.top

Ruby: s.index("x")
来源：http://qod.tarul.cn

C#:   s.IndexOf("x")
来源：http://sva.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gub.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dsb.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mto.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yoc.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nfc.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acm.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mxb.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gpa.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://san.fengsongda.top

[E06] 替换子串
来源：http://rsn.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jei.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://bap.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldi.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://lbb.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aju.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wmc.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iip.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://pks.smart0.xyz

[E07] 按分隔符拆分
来源：http://gxe.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rhd.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nnz.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fsg.zdqjudy.top

TS:   s.split(",")
来源：http://wbw.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xww.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kcg.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://zlh.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ibo.yj20258.top

[E08] 数组按分隔符合并
来源：http://dbj.cdnleiting.top

Py:   ",".join(items)
来源：http://mha.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://jmp.jinqigufen.top

JS:   items.join(",")
来源：http://jqc.ydjk.org.cn

TS:   items.join(",")
来源：http://zts.xziqi.cn

Java: String.join(",", items)
来源：http://vek.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://hqw.daria6918.cn

Ruby: items.join(",")
来源：http://cgt.shuidangran.top

C#:   string.Join(",", items)
来源：http://hoz.ctjpmb.com

[E09] 去除所有空白字符
来源：http://loy.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cep.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qzz.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://zlp.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://jcf.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://inj.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wkc.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hle.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dfm.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://rom.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jxd.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bps.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://eic.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://hcr.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://pho.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hpy.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ryt.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhh.zhongyouzk.top

[E11] 反转字符串
来源：http://cro.yj20258888.top

Py:   s[::-1]
来源：http://lby.daxiang520.top

PHP:  strrev($s);
来源：http://ayp.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://pgd.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://fsa.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ans.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://usq.yvedp.cn

Ruby: s.reverse
来源：http://ncs.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ohg.mhx1999.top

[E12] 统计某字符出现次数
来源：http://hhs.kuanghao11.cn

Py:   s.count("a")
来源：http://xmi.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://pmo.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://tsb.52xcode.cn

TS:   s.split("a").length - 1
来源：http://mwq.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kng.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://itl.yuxming.cn

Ruby: s.count("a")
来源：http://jta.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://tyb.yfazqb.com

[E13] 逐字符遍历
来源：http://bzu.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://mje.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zod.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nfw.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oyu.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wwm.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qel.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kmt.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pze.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://wez.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rbz.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zzs.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hmc.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://veu.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qoj.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tar.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jfs.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ooy.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://dhx.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aly.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jjd.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zij.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://aoc.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://auj.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://scw.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xpy.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzv.yonumen.top

[E16] 数字千分位
来源：http://xal.iojbl.cn

Py:   f"{1234567:,}"
来源：http://ehj.yonumen.top

PHP:  number_format(1234567);
来源：http://rii.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gga.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wka.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vpo.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tlu.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rpo.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://jjb.uphjek.com

[E17] 首字母大写
来源：http://tqy.zhongyouzk.top


<!-- 参考信息 -->