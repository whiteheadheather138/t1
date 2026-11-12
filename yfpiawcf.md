代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yvq.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqr.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://isk.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxj.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fbv.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ohl.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://brv.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jcp.guowangkeji.top

[D11] 反转数组
来源：http://pfl.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://vid.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://nqf.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wvf.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://lxd.daria6918.cn

Java: Collections.reverse(list);
来源：http://qck.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://mus.tian-w.cn

Ruby: arr.reverse
来源：http://wjh.tanke756.top

C#:   list.Reverse();
来源：http://tiq.hysaishi.cn

[D12] 查找元素下标
来源：http://jhl.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://qwf.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nqv.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xce.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hna.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ged.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://pxx.jqgfzy.top

Ruby: arr.index(x)
来源：http://dya.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://uoc.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://ryn.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qgh.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hog.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://qdx.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://msn.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wtx.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gfx.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://nyj.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zml.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://xnm.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sml.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kgr.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://ave.sweek.top

TS:   arr.map(x => x * 2)
来源：http://yyj.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vds.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://txv.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://fjg.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mtv.cucudq.cn

[D15] 去重
来源：http://vth.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cqd.cucudq.cn

PHP:  array_unique($arr);
来源：http://sep.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://fmv.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://rrl.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ict.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://vte.yuxming.cn

Ruby: arr.uniq
来源：http://shm.meibo888.top

C#:   list.Distinct().ToList()
来源：http://bzm.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://rso.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ltf.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tgn.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iji.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcr.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fnk.jinqigfzy.top

Go:   // 手写循环累加
来源：http://eav.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gpx.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://nre.cdnleiting.top

[D17] 最大值与最小值
来源：http://cjs.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://rqf.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://ofn.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iuv.birdmap.top

TS:   Math.max(...arr);
来源：http://kuw.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jda.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://znq.yonumen.top

Ruby: arr.max;  arr.min
来源：http://wjt.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://dof.pycfn.com

[D18] 扁平化嵌套数组
来源：http://gtg.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://siv.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://qpp.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zku.andypj.xyz

TS:   nested.flat();
来源：http://mdc.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rbm.52xcode.cn

Go:   // 手写双层循环
来源：http://eyc.uphjek.com

Ruby: nested.flatten
来源：http://hez.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qhs.yj20258.top

[D19] 按字段分组
来源：http://biz.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oji.chenjidiqi.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hzj.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yht.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://zdi.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qji.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://khy.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ikc.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lsm.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://ljw.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://dka.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://dgr.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fwk.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fau.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://usr.yfazqb.com

Go:   // 手写 map[T]int
来源：http://bhi.shangyingyoupin.top

Ruby: arr.tally
来源：http://xdj.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ous.hammf.cn

[D21] 判断是否包含某元素
来源：http://vuq.xuetiantiany.cn

Py:   x in arr
来源：http://rbq.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://xua.daria6918.cn

JS:   arr.includes(x)
来源：http://jjk.jlsjyb.cn

TS:   arr.includes(x)
来源：http://iyk.nanxuanxn.top

Java: list.contains(x)
来源：http://upc.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://vob.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://awp.xuanzx.com

C#:   list.Contains(x)
来源：http://sig.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://vab.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hvm.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iof.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vsq.fzhhl.top

TS:   [...arr];
来源：http://eud.andypj.xyz

Java: new ArrayList<>(list);
来源：http://oux.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gjl.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://tuz.bjfxy.top

C#:   new List<int>(list);
来源：http://prr.jqgufenzy.top

[D23] reduce 累积计算
来源：http://ngh.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vdd.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tqs.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xah.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxu.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://gxa.chenjidiqi.icu

Go:   // 手写循环
来源：http://fji.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mto.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://klr.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://vio.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://big.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dns.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xyk.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aah.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujl.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cub.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rez.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://enw.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://lzh.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uan.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qid.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qgj.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rcj.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ptj.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rfq.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://okq.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fhu.sjlbkw.cn

[D26] 数组转字符串
来源：http://vlj.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://yun.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://ceq.zycfv.cn

JS:   arr.join(", ")
来源：http://zmr.sysykeji.top

TS:   arr.join(", ")
来源：http://und.zhijiandao.cn

Java: String.join(", ", list)
来源：http://fqh.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://ipr.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://fxb.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://sgt.fehbvm.com

================================================================================
来源：http://nnq.feifeiyinyue.top

E. 字符串处理
来源：http://owx.jlsjyb.cn

================================================================================
来源：http://qua.yj202588.top

[E01] 拼接字符串
来源：http://zte.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tgl.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rvo.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zka.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oco.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://izc.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dxa.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bvd.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ujh.zdqjudy.top

[E02] 重复字符串
来源：http://izh.epnwcf.com

Py:   "ab" * 3
来源：http://pcw.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://zrl.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://yri.c1oappe.top

TS:   "ab".repeat(3)
来源：http://tle.yueranfly.top

Java: "ab".repeat(3)
来源：http://ala.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://meb.gaohongyu789.top

Ruby: "ab" * 3
来源：http://gwv.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://apy.sxryk.cn

[E03] 截取子串
来源：http://pxj.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ogj.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bgr.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://auz.daria6918.cn

TS:   s.slice(1, 4)
来源：http://ikl.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://xjv.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://knz.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://jnh.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://ggz.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://dpy.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://apk.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://brl.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qvv.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://cqb.gogol.net.cn

Java: s.indexOf("x")
来源：http://wbf.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://dvm.ybcxt.top

Ruby: s.index("x")
来源：http://hfz.yj20258888.top

C#:   s.IndexOf("x")
来源：http://gbi.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pyk.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://klk.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yop.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgz.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://chs.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ibr.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ers.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pln.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ffj.epnwcf.com

[E06] 替换子串
来源：http://vtn.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rja.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://vfj.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tou.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://cgb.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xae.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://thz.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://htt.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://mgs.bjfxy.top

[E07] 按分隔符拆分
来源：http://fwj.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://buw.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pxq.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nvk.jinghuilouyu.cn

TS:   s.split(",")
来源：http://yek.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zox.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tnv.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://egm.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ghu.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://mmx.kuanghao11.cn

Py:   ",".join(items)
来源：http://hed.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://ylx.fzhhl.top

JS:   items.join(",")
来源：http://tgw.sufxvd.cn

TS:   items.join(",")
来源：http://ewp.yanxiufei.cn

Java: String.join(",", items)
来源：http://bhe.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://dpk.wangdashe.top

Ruby: items.join(",")
来源：http://duu.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://yge.52xcode.cn

[E09] 去除所有空白字符
来源：http://kjs.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tzw.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ooa.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://ldw.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://box.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://rcb.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dfq.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://zip.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tmp.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://yiv.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mty.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yyg.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://pow.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://nap.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://ohj.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yqc.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bfg.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://voe.jinqigfzy.top

[E11] 反转字符串
来源：http://wim.kuanghao11.cn

Py:   s[::-1]
来源：http://djm.yuxming.cn

PHP:  strrev($s);
来源：http://sow.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://cef.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://hlg.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dph.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgw.hammf.cn

Ruby: s.reverse
来源：http://udw.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://wml.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://zwn.jyoumei.cn

Py:   s.count("a")
来源：http://lbq.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://tpp.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://oxd.sysykeji.top

TS:   s.split("a").length - 1
来源：http://ptq.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qyl.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://wwy.gotoacloud.top

Ruby: s.count("a")
来源：http://jze.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://rtl.bbcook.cn

[E13] 逐字符遍历
来源：http://kmg.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://sna.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://piz.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://eqy.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wvd.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gey.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ige.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sqi.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zfz.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://rvm.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lwa.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mrc.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hpa.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vml.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jne.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tna.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hlr.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eot.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://rek.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ktd.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eip.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vaz.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qkv.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rjw.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qqu.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://slb.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vwr.guowangkeji.top

[E16] 数字千分位
来源：http://esd.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://vzt.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://hxx.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jvk.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rqd.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ssk.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zis.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://civ.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://mas.ydjk.org.cn

[E17] 首字母大写
来源：http://ifc.sufxvd.cn


<!-- 参考信息 -->