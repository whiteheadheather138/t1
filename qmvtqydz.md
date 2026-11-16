代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://heu.sjlbkw.cn

Ruby: arr.sort
来源：http://swz.shanyushiyangtech.top

C#:   list.Sort();
来源：http://ybn.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://egy.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sre.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ugw.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eyr.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iot.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbj.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rna.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jfp.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rmq.9152youxi.cn

[D11] 反转数组
来源：http://khn.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dco.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://ahd.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://auh.jinqigufen.top

TS:   [...arr].reverse();
来源：http://wrl.bbcook.cn

Java: Collections.reverse(list);
来源：http://krr.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://psf.sysykeji.top

Ruby: arr.reverse
来源：http://dba.tarul.cn

C#:   list.Reverse();
来源：http://nge.zhengqikj.top

[D12] 查找元素下标
来源：http://khi.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://rai.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbg.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gps.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jst.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tcm.birdmap.top

Go:   slices.Index(arr, x)
来源：http://nqu.epnwcf.com

Ruby: arr.index(x)
来源：http://ugt.vehdjk.com

C#:   list.IndexOf(x);
来源：http://tsw.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://kle.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ecn.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qjt.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://uti.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://gam.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://awl.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xsd.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://vqq.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://onx.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://aep.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tem.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iad.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://zxb.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://fow.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rhy.gzhubu.top

Go:   // 手写循环
来源：http://csz.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://bkl.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://njy.chenzaomai.com

[D15] 去重
来源：http://ypf.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ioj.dianchejie.cn

PHP:  array_unique($arr);
来源：http://hcd.daxiang520.top

JS:   [...new Set(arr)]
来源：http://aci.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://ssf.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xbk.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://ztd.cheryme.top

Ruby: arr.uniq
来源：http://ium.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://rdg.yangfankeji.com

[D16] 求和与平均值
来源：http://ubh.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vds.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kgq.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sim.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rla.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://scs.ydzc1.top

Go:   // 手写循环累加
来源：http://rga.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://maj.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://xvc.yuanzhike.top

[D17] 最大值与最小值
来源：http://dea.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://xho.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://vkz.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kqk.cheryme.top

TS:   Math.max(...arr);
来源：http://egk.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tbw.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cds.havefunace.top

Ruby: arr.max;  arr.min
来源：http://gpm.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://mew.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://cne.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mfh.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://tgj.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sjd.vqdsnc.cn

TS:   nested.flat();
来源：http://anm.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lga.yueranfly.top

Go:   // 手写双层循环
来源：http://bje.shzxlz.cn

Ruby: nested.flatten
来源：http://rcv.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tge.ivvv.top

[D19] 按字段分组
来源：http://dgi.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lzv.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pnh.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://obm.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wjh.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vou.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://kpi.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gml.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wke.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://jal.fehbvm.com

Py:   Counter(arr)
来源：http://frp.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nuk.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nun.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jon.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jjy.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://zpx.chenjidiqi.icu

Ruby: arr.tally
来源：http://ohp.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://arl.uphjek.com

[D21] 判断是否包含某元素
来源：http://xag.ydjk.org.cn

Py:   x in arr
来源：http://jnl.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://uux.iojbl.cn

JS:   arr.includes(x)
来源：http://jee.ydjk.org.cn

TS:   arr.includes(x)
来源：http://inu.guowangkeji.top

Java: list.contains(x)
来源：http://ryy.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://aox.gogol.net.cn

Ruby: arr.include?(x)
来源：http://ndr.wangdashe.top

C#:   list.Contains(x)
来源：http://gtj.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://cqf.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://inq.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ucp.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tky.cashguo.top

TS:   [...arr];
来源：http://ncs.xinyue.icu

Java: new ArrayList<>(list);
来源：http://owy.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://ikh.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://bqh.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://nng.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://omo.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://byc.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tch.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iiu.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yhy.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://myw.jqgufenzy.top

Go:   // 手写循环
来源：http://roa.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fod.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jeo.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://nms.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://slh.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ekk.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rvq.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ngn.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xli.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rpq.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hsp.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hah.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://yay.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cpj.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://chw.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://arw.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ikk.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nta.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://whp.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ilk.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ric.nwbrower.top

[D26] 数组转字符串
来源：http://ojz.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://ank.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://fts.yonumen.top

JS:   arr.join(", ")
来源：http://udr.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://ltw.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://uot.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://msd.tianlin.xyz

Ruby: arr.join(", ")
来源：http://ngf.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://ceh.xingfuxueyuan.xyz

================================================================================
来源：http://fbw.pycfn.com

E. 字符串处理
来源：http://hvf.daria6918.cn

================================================================================
来源：http://cgi.hongshengwenyu.top

[E01] 拼接字符串
来源：http://hnx.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bfl.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dxk.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnx.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyi.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wvn.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://urb.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hip.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://stq.xuetiantiany.cn

[E02] 重复字符串
来源：http://avu.aizwys.cn

Py:   "ab" * 3
来源：http://zmu.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://lem.yvedp.cn

JS:   "ab".repeat(3)
来源：http://pay.fzhhl.top

TS:   "ab".repeat(3)
来源：http://vxr.gotoacloud.top

Java: "ab".repeat(3)
来源：http://ltx.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://afp.quarkkingdee.top

Ruby: "ab" * 3
来源：http://qkp.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://exw.cqqwz.cn

[E03] 截取子串
来源：http://mvd.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cmi.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwk.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ext.yj202588.top

TS:   s.slice(1, 4)
来源：http://dha.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://nun.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dym.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://slx.yongpay.top

C#:   s.Substring(1, 3)
来源：http://vxl.feifeiyinyue.top

[E04] 查找子串位置
来源：http://bay.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://pzu.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://uth.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qmw.sysykeji.top

TS:   s.indexOf("x")
来源：http://sdr.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://ayi.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://cho.ppjwa.cn

Ruby: s.index("x")
来源：http://nzg.sxryk.cn

C#:   s.IndexOf("x")
来源：http://sot.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nht.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://upl.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xrb.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://slm.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vds.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvz.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vnh.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://izz.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjx.hywenlv.cn

[E06] 替换子串
来源：http://vsd.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pnp.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://mmz.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rko.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://sll.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ilb.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zhe.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygh.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://pvq.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://ymh.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://med.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mzp.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jxg.fzhhl.top

TS:   s.split(",")
来源：http://xni.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://ygp.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gyo.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://raz.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yyv.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://zuk.tarul.cn

Py:   ",".join(items)
来源：http://hdp.jiagoushi.top

PHP:  implode(",", $items);
来源：http://bmi.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://opj.cashguo.top

TS:   items.join(",")
来源：http://gqh.shuidangran.top

Java: String.join(",", items)
来源：http://ttf.yj20258.top

Go:   strings.Join(items, ",")
来源：http://wcx.vqdsnc.cn

Ruby: items.join(",")
来源：http://hwn.xuanzx.com

C#:   string.Join(",", items)
来源：http://bwi.vehdjk.com

[E09] 去除所有空白字符
来源：http://otd.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctk.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kbr.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://aqq.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://rrg.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://cca.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mvp.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cyv.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rlt.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://yru.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nhp.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gia.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://vkn.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://xcl.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://qjg.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pun.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eym.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yhq.shzxlz.cn

[E11] 反转字符串
来源：http://wja.zhongyouzk.top

Py:   s[::-1]
来源：http://wml.gogol.net.cn

PHP:  strrev($s);
来源：http://odf.ivvv.top

JS:   [...s].reverse().join("")
来源：http://cfd.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://byi.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pfz.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://suo.zhoulong.xyz

Ruby: s.reverse
来源：http://dgy.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://npm.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://lnf.yuanzhike.top

Py:   s.count("a")
来源：http://pxf.havefunace.top

PHP:  substr_count($s, "a");
来源：http://qoj.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://wke.tian-w.cn

TS:   s.split("a").length - 1
来源：http://fhw.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qeh.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://ksf.aibaodan.cn

Ruby: s.count("a")
来源：http://dvz.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://usy.sweek.top

[E13] 逐字符遍历
来源：http://kbu.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://fka.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ynx.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gjh.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gws.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zyz.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yey.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://utv.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dtd.ybcxt.top

[E14] URL 编码与 Base64
来源：http://jsq.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gud.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mii.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwl.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hso.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tik.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ggq.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gob.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kgi.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://fwc.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bxc.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ear.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bdz.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yac.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jjl.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mhm.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sux.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://spl.chenzaomai.com

[E16] 数字千分位
来源：http://bop.fzhhl.top

Py:   f"{1234567:,}"
来源：http://efe.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://vpv.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xbw.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://owk.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://spf.yuxming.cn


<!-- 参考信息 -->