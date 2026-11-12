代发 wailian999

PHP:  sort($arr);
来源：http://cua.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gjd.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://egb.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://asj.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cfc.sxryk.cn

Ruby: arr.sort
来源：http://jkt.yvedp.cn

C#:   list.Sort();
来源：http://fzn.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xfl.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pmd.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twc.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejy.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxu.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://utu.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qxp.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://enq.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ywe.smart0.xyz

[D11] 反转数组
来源：http://qaa.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://apn.yueranfly.top

PHP:  array_reverse($arr);
来源：http://fqg.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kas.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://pbf.ehwqpu.com

Java: Collections.reverse(list);
来源：http://qap.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://jee.yj20258.top

Ruby: arr.reverse
来源：http://vnn.daria6918.cn

C#:   list.Reverse();
来源：http://bds.yueranfly.top

[D12] 查找元素下标
来源：http://jag.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://tpe.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nqo.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vum.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shy.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oef.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://mkf.nanxuanxn.top

Ruby: arr.index(x)
来源：http://jwt.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://njl.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://bnp.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vyh.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ehe.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://oxu.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://eup.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ftm.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rlz.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://sou.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://itn.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://wfr.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imp.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oqz.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://otu.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://tck.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lfd.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://gou.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kwl.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zsi.dashuyun.cn

[D15] 去重
来源：http://woz.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oow.sysykeji.top

PHP:  array_unique($arr);
来源：http://yar.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://jdd.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://mcl.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mua.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://uvy.snrcjt.cn

Ruby: arr.uniq
来源：http://kjy.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://vqw.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://ube.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wqm.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mey.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jlf.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxh.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cfs.zycfv.cn

Go:   // 手写循环累加
来源：http://hrr.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkr.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://sfk.hesvh.cn

[D17] 最大值与最小值
来源：http://vxj.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://wkm.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://gva.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ufm.yuanzhike.top

TS:   Math.max(...arr);
来源：http://adz.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cet.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lnf.cheryme.top

Ruby: arr.max;  arr.min
来源：http://dqj.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://gko.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://gmc.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fdo.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://mzr.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://izg.wangshuangyany.cn

TS:   nested.flat();
来源：http://biu.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://amo.bjfxy.top

Go:   // 手写双层循环
来源：http://zri.tanke756.top

Ruby: nested.flatten
来源：http://aia.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ymf.hysaishi.cn

[D19] 按字段分组
来源：http://med.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hhc.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cct.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://phq.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qhj.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://stz.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://hqo.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://neg.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jpf.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://kfn.epnwcf.com

Py:   Counter(arr)
来源：http://azq.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://ybg.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvk.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsj.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zha.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://hlu.yangfankeji.com

Ruby: arr.tally
来源：http://hqr.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hlt.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://zpr.kuanghao11.cn

Py:   x in arr
来源：http://dct.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://ims.chenlongwang.top

JS:   arr.includes(x)
来源：http://wdx.52xcode.cn

TS:   arr.includes(x)
来源：http://kqc.sufxvd.cn

Java: list.contains(x)
来源：http://een.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://uuz.zdqjudy.top

Ruby: arr.include?(x)
来源：http://toi.cucudq.cn

C#:   list.Contains(x)
来源：http://rop.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://nff.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wnm.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ual.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gfd.sweek.top

TS:   [...arr];
来源：http://ojv.xinyue.icu

Java: new ArrayList<>(list);
来源：http://ctv.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://dox.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://ynx.guannengcc.top

C#:   new List<int>(list);
来源：http://ozc.jinqigfzy.top

[D23] reduce 累积计算
来源：http://ufd.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zdw.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://imh.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ltw.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omj.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://das.jianghu66.top

Go:   // 手写循环
来源：http://cvt.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://onv.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pnp.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://qga.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gtw.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bjo.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://beo.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xma.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nrd.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ylv.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ckc.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vpz.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://cyo.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gdn.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sps.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zbu.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dct.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jtg.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xzu.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qmh.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oxn.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://asl.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://fhs.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://rtv.chenlongwang.top

JS:   arr.join(", ")
来源：http://coy.tian-w.cn

TS:   arr.join(", ")
来源：http://nrq.havefunace.top

Java: String.join(", ", list)
来源：http://bjm.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://nwl.xziqi.cn

Ruby: arr.join(", ")
来源：http://cab.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://xjs.yvedp.cn

================================================================================
来源：http://dgh.guannengcc.top

E. 字符串处理
来源：http://lhu.shanyushiyangtech.top

================================================================================
来源：http://ipe.snrcjt.cn

[E01] 拼接字符串
来源：http://bvy.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgm.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wbr.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yvp.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gxy.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eim.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gld.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qan.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hbo.hywenlv.cn

[E02] 重复字符串
来源：http://fbm.sweek.top

Py:   "ab" * 3
来源：http://owm.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://ahn.hesvh.cn

JS:   "ab".repeat(3)
来源：http://jiw.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://xyn.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://mdp.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://tlg.yueranfly.top

Ruby: "ab" * 3
来源：http://kxg.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pwf.sjlbkw.cn

[E03] 截取子串
来源：http://rzl.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zoa.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hhf.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ycw.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://jay.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://but.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://urd.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fys.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://oyc.dianchejie.cn

[E04] 查找子串位置
来源：http://zdl.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://rze.sxryk.cn

PHP:  strpos($s, "x");
来源：http://odh.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jnq.yuanzhike.top

TS:   s.indexOf("x")
来源：http://ynp.cucudq.cn

Java: s.indexOf("x")
来源：http://qbc.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://zzh.xuanzx.com

Ruby: s.index("x")
来源：http://ovg.cucudq.cn

C#:   s.IndexOf("x")
来源：http://mlr.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tmd.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://que.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fev.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfs.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xiu.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aep.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://idz.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cld.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xjd.aibaodan.cn

[E06] 替换子串
来源：http://ony.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mnu.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://zxb.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yde.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://zpk.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcq.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oun.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://isg.yongpay.top

C#:   s.Replace("a", "b")
来源：http://zew.zycfv.cn

[E07] 按分隔符拆分
来源：http://tuc.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dap.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cgb.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jxl.wangshuangyany.cn

TS:   s.split(",")
来源：http://ckh.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://ujr.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mvg.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://xbj.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ypr.andypj.xyz

[E08] 数组按分隔符合并
来源：http://eit.zhoulong.xyz

Py:   ",".join(items)
来源：http://jff.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://qhb.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://asl.dashuyun.cn

TS:   items.join(",")
来源：http://ipz.birdmap.top

Java: String.join(",", items)
来源：http://hbg.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://tqt.andypj.xyz

Ruby: items.join(",")
来源：http://jcw.xylfe.cn

C#:   string.Join(",", items)
来源：http://izd.yvedp.cn

[E09] 去除所有空白字符
来源：http://bys.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kld.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yju.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://mhu.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://tct.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://qhp.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://chv.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kuc.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nog.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://sxa.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qww.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lyk.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://qrd.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://brm.guannengcc.top

Java: String.format("%03d", 7)
来源：http://iws.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zqu.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://omw.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aed.hnxiangtu.top

[E11] 反转字符串
来源：http://ajb.birdmap.top

Py:   s[::-1]
来源：http://cjz.sysykeji.top

PHP:  strrev($s);
来源：http://fvr.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://uud.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://wen.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wvr.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mzd.andypj.xyz

Ruby: s.reverse
来源：http://vwf.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://egr.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://jbi.fehbvm.com

Py:   s.count("a")
来源：http://spg.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://srd.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://udw.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://odi.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azt.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://erl.gogol.net.cn

Ruby: s.count("a")
来源：http://lvw.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://thw.cheryme.top

[E13] 逐字符遍历
来源：http://vyq.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://zgf.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://etz.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ptk.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uzb.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ydf.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bvf.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ijj.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vop.iojbl.cn

[E14] URL 编码与 Base64
来源：http://xxs.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pmz.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mtc.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jtl.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hcc.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bva.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tbj.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbg.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oqa.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://xyy.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pnk.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://htc.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lni.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://uhy.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aho.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dit.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ncq.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jro.hcnkem.com

[E16] 数字千分位
来源：http://esk.hnqzz.top

Py:   f"{1234567:,}"
来源：http://qcs.gaohongyu789.top


<!-- 参考信息 -->