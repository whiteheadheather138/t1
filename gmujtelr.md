代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://byh.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gzv.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ebq.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://skx.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bbt.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rdv.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhj.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wje.shzxlz.cn

[D11] 反转数组
来源：http://goj.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://izv.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://ywn.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://txf.jyoumei.cn

TS:   [...arr].reverse();
来源：http://pzv.cheryme.top

Java: Collections.reverse(list);
来源：http://hnu.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://uxs.zdqjudy.top

Ruby: arr.reverse
来源：http://zto.feifeiyinyue.top

C#:   list.Reverse();
来源：http://ulp.hywenlv.cn

[D12] 查找元素下标
来源：http://bun.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://dtu.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gvm.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbr.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gwi.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mry.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://ilk.shuidangran.top

Ruby: arr.index(x)
来源：http://zfu.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://erk.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://msp.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ljy.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xes.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://ccf.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://opa.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vqd.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pzd.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://viz.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kaa.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://nkn.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hef.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wft.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://woj.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://rlg.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fpy.zhongyouzk.top

Go:   // 手写循环
来源：http://awo.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://xke.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xxf.xuanzx.com

[D15] 去重
来源：http://let.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jtc.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://gwl.yvedp.cn

JS:   [...new Set(arr)]
来源：http://glt.bbcook.cn

TS:   [...new Set(arr)]
来源：http://jei.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eef.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://gml.chenzaomai.com

Ruby: arr.uniq
来源：http://wtn.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://eno.birdmap.top

[D16] 求和与平均值
来源：http://rxg.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ldo.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ljo.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cha.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aey.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rez.meibo888.top

Go:   // 手写循环累加
来源：http://rzc.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://okq.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://ocz.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://mdi.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://ypr.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://sfw.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://glt.daxiang520.top

TS:   Math.max(...arr);
来源：http://wha.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kyb.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hzv.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://kvv.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://mbt.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://ogo.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibj.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://unl.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kvo.yuanzhike.top

TS:   nested.flat();
来源：http://ufu.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nue.chenlongwang.top

Go:   // 手写双层循环
来源：http://bkq.yongpay.top

Ruby: nested.flatten
来源：http://omg.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nen.redwolf501.top

[D19] 按字段分组
来源：http://usp.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tmn.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cad.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wms.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vva.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vky.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://zzr.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://jcq.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pwh.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://xdb.yonumen.top

Py:   Counter(arr)
来源：http://ghs.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://qcb.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://csm.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cej.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ykt.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://btb.cucudq.cn

Ruby: arr.tally
来源：http://jbl.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onf.bbcook.cn

[D21] 判断是否包含某元素
来源：http://dng.wangdashe.top

Py:   x in arr
来源：http://tpc.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://tzx.epnwcf.com

JS:   arr.includes(x)
来源：http://qip.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://hud.ppjwa.cn

Java: list.contains(x)
来源：http://hor.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://zmj.andypj.xyz

Ruby: arr.include?(x)
来源：http://hqa.fengsongda.top

C#:   list.Contains(x)
来源：http://hfl.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://iqk.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axp.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://frt.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://weq.tian-w.cn

TS:   [...arr];
来源：http://tkl.cucudq.cn

Java: new ArrayList<>(list);
来源：http://hhg.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lxp.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://yyj.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://ypq.hammf.cn

[D23] reduce 累积计算
来源：http://giz.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ffc.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzu.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxv.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kfw.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kkd.zhixingplan.top

Go:   // 手写循环
来源：http://kss.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://juo.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://boa.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://mun.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mga.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wns.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xfp.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://czm.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgs.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzu.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nha.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hsz.tanke756.top

[D25] Set 集合去重与交并差
来源：http://qry.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ayn.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iqw.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qui.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cyv.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gyr.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tez.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vnl.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://faw.gotoacloud.top

[D26] 数组转字符串
来源：http://tpz.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://ylz.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://kzm.9152youxi.cn

JS:   arr.join(", ")
来源：http://svm.ydzc1.top

TS:   arr.join(", ")
来源：http://lqx.dianchejie.cn

Java: String.join(", ", list)
来源：http://gvn.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://ffg.epnwcf.com

Ruby: arr.join(", ")
来源：http://jvr.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://otc.snrcjt.cn

================================================================================
来源：http://dhf.aibaodan.cn

E. 字符串处理
来源：http://ozt.zhengqikj.top

================================================================================
来源：http://huv.nanxinkj.top

[E01] 拼接字符串
来源：http://fjq.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zjw.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://adc.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://seb.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://imr.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mrm.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hcr.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pqq.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://miv.feifeiyinyue.top

[E02] 重复字符串
来源：http://ysd.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://jkk.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://wkb.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://ici.andypj.xyz

TS:   "ab".repeat(3)
来源：http://pmu.cheryme.top

Java: "ab".repeat(3)
来源：http://afj.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://nno.guannengcc.top

Ruby: "ab" * 3
来源：http://scf.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bcs.hnqzz.top

[E03] 截取子串
来源：http://xmb.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xai.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rqn.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xfm.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://zfq.cdnleiting.top

Java: s.substring(1, 4)
来源：http://oni.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://amt.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://bvu.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://ymw.nanxuanxn.top

[E04] 查找子串位置
来源：http://tgl.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://hzo.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://lct.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://imr.52xcode.cn

TS:   s.indexOf("x")
来源：http://zba.wangdashe.top

Java: s.indexOf("x")
来源：http://kxp.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://fgw.hysaishi.cn

Ruby: s.index("x")
来源：http://iti.epnwcf.com

C#:   s.IndexOf("x")
来源：http://rvf.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ixd.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itt.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hge.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgu.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ndf.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdn.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dbn.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwy.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gjy.vqdsnc.cn

[E06] 替换子串
来源：http://ioq.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://elj.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://osx.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgo.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://klx.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxl.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ira.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pvy.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://nid.cqqwz.cn

[E07] 按分隔符拆分
来源：http://ddi.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tbz.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hjb.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xmi.kuanghao11.cn

TS:   s.split(",")
来源：http://ekg.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://ehs.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iei.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://sbf.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vhz.daria6918.cn

[E08] 数组按分隔符合并
来源：http://xjr.guowangkeji.top

Py:   ",".join(items)
来源：http://sff.aizwys.cn

PHP:  implode(",", $items);
来源：http://lhs.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://zuf.birdmap.top

TS:   items.join(",")
来源：http://epl.daria6918.cn

Java: String.join(",", items)
来源：http://qzv.hammf.cn

Go:   strings.Join(items, ",")
来源：http://cbt.jiagoushi.top

Ruby: items.join(",")
来源：http://svt.jyoumei.cn

C#:   string.Join(",", items)
来源：http://dna.xziqi.cn

[E09] 去除所有空白字符
来源：http://mvv.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gkw.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xoh.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://kfh.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://gto.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://bbi.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vzh.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://xwc.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tuu.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://nxi.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fad.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://trj.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://awi.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://dgq.nwbrower.top

Java: String.format("%03d", 7)
来源：http://dwh.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zur.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fbr.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyx.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://fsd.jianghu66.top

Py:   s[::-1]
来源：http://rjm.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://omg.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://nke.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://sjq.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nqm.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzs.wangshuangyany.cn

Ruby: s.reverse
来源：http://eel.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://bqq.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://yli.fktsv.cn

Py:   s.count("a")
来源：http://kft.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://zxw.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://plu.wangdashe.top

TS:   s.split("a").length - 1
来源：http://jvm.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://esf.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://jmq.ydzc1.top

Ruby: s.count("a")
来源：http://kqm.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://zyl.nwbrower.top

[E13] 逐字符遍历
来源：http://kok.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://jdb.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mnn.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ozo.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kjb.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qev.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bbh.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nku.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fyo.xziqi.cn

[E14] URL 编码与 Base64
来源：http://hfm.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yuj.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eih.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjl.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cmb.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qnb.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aki.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qck.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://upf.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://rqm.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ovm.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ols.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pjx.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fxw.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cce.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mue.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ksd.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://brz.dianchejie.cn

[E16] 数字千分位
来源：http://uky.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://wmm.hnqzz.top

PHP:  number_format(1234567);
来源：http://hdb.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hla.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tgv.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eve.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gtw.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zqb.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://cdk.yvedp.cn

[E17] 首字母大写
来源：http://lyc.xuetiantiany.cn


<!-- 参考信息 -->