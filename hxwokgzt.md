代发 wailian999

PHP:  sort($arr);
来源：http://rhm.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qqf.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sfs.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vin.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://woh.pycfn.com

Ruby: arr.sort
来源：http://wjj.snrcjt.cn

C#:   list.Sort();
来源：http://hlt.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://bcr.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wyx.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tse.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbj.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ptf.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nxk.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://spj.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nlw.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ecr.zhijiandao.cn

[D11] 反转数组
来源：http://tny.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ccb.c1oappe.top

PHP:  array_reverse($arr);
来源：http://age.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://juq.tarul.cn

TS:   [...arr].reverse();
来源：http://lil.meibo888.top

Java: Collections.reverse(list);
来源：http://lcf.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://hvv.ydjk.org.cn

Ruby: arr.reverse
来源：http://rge.cqqwz.cn

C#:   list.Reverse();
来源：http://gwz.chenlongwang.top

[D12] 查找元素下标
来源：http://efu.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://imd.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ltb.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwb.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhc.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://imp.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://mcp.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://kxc.c1oappe.top

C#:   list.IndexOf(x);
来源：http://pri.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://mdf.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kkh.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lau.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://lvs.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://pno.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://slo.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://twq.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://imi.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mwy.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://grs.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ytt.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kfe.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://vjd.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://iup.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pyz.fanxiaobao.xyz

Go:   // 手写循环
来源：http://ryn.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://woi.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rva.gotoacloud.top

[D15] 去重
来源：http://ipr.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://per.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://pgz.meibo888.top

JS:   [...new Set(arr)]
来源：http://mcn.uphjek.com

TS:   [...new Set(arr)]
来源：http://vba.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xih.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dmh.zhengqikj.top

Ruby: arr.uniq
来源：http://jkq.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://ffg.chenlongwang.top

[D16] 求和与平均值
来源：http://mhc.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wev.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://szm.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qia.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cib.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gzq.haohaochexian.top

Go:   // 手写循环累加
来源：http://tfa.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xxw.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://fmv.sufxvd.cn

[D17] 最大值与最小值
来源：http://mal.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://hof.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://not.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://frf.redwolf501.top

TS:   Math.max(...arr);
来源：http://mmk.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://psj.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bra.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://hcf.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://fce.meibo888.top

[D18] 扁平化嵌套数组
来源：http://bco.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://epm.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://mrc.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rfl.sufxvd.cn

TS:   nested.flat();
来源：http://wcy.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozb.nanxuanxn.top

Go:   // 手写双层循环
来源：http://fkc.chenlongwang.top

Ruby: nested.flatten
来源：http://kza.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zap.smart0.xyz

[D19] 按字段分组
来源：http://hpl.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ywr.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pnj.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uhy.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://usz.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzy.redwolf501.top

Go:   // 手写 map[string][]T
来源：http://ash.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://nxt.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mek.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://gzj.gzhubu.top

Py:   Counter(arr)
来源：http://frw.birdmap.top

PHP:  array_count_values($arr);
来源：http://mlv.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nll.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqv.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oqa.birdmap.top

Go:   // 手写 map[T]int
来源：http://mpf.yangfankeji.com

Ruby: arr.tally
来源：http://sdo.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wif.xinyue.icu

[D21] 判断是否包含某元素
来源：http://vmh.bbcook.cn

Py:   x in arr
来源：http://prm.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://pzc.fktsv.cn

JS:   arr.includes(x)
来源：http://acm.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://gwz.aibaodan.cn

Java: list.contains(x)
来源：http://hgm.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://jen.bbcook.cn

Ruby: arr.include?(x)
来源：http://tks.andypj.xyz

C#:   list.Contains(x)
来源：http://gzv.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://equ.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bng.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jsh.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qoe.shuidangran.top

TS:   [...arr];
来源：http://ukz.hcnkem.com

Java: new ArrayList<>(list);
来源：http://fwf.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://xco.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://vuq.zycfv.cn

C#:   new List<int>(list);
来源：http://ttd.guowangkeji.top

[D23] reduce 累积计算
来源：http://tyn.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sfq.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://abp.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iwa.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jju.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zag.zhongyouzk.top

Go:   // 手写循环
来源：http://fnj.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uqg.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bqh.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://yhd.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jnx.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://goa.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rcm.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qyu.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bmt.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hzw.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pom.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oro.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://rmf.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nne.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bmj.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftb.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rhq.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zen.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bqe.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xqd.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sud.zhoulong.xyz

[D26] 数组转字符串
来源：http://yjg.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://hlq.uphjek.com

PHP:  implode(", ", $arr);
来源：http://kfk.jinqigufen.top

JS:   arr.join(", ")
来源：http://uac.yuxming.cn

TS:   arr.join(", ")
来源：http://nrp.epnwcf.com

Java: String.join(", ", list)
来源：http://gjv.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://mfy.meibo888.top

Ruby: arr.join(", ")
来源：http://nca.52xcode.cn

C#:   string.Join(", ", list)
来源：http://xym.ydjk.org.cn

================================================================================
来源：http://ewp.zhengqikj.top

E. 字符串处理
来源：http://fja.aizwys.cn

================================================================================
来源：http://afn.guowangkeji.top

[E01] 拼接字符串
来源：http://rth.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nhr.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjy.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcw.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddn.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oto.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iow.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://csh.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eor.fehbvm.com

[E02] 重复字符串
来源：http://icf.daxiang520.top

Py:   "ab" * 3
来源：http://zbx.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://aww.hesvh.cn

JS:   "ab".repeat(3)
来源：http://wcp.jianghu66.top

TS:   "ab".repeat(3)
来源：http://xot.jianghu66.top

Java: "ab".repeat(3)
来源：http://cbn.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://qre.zhoulong.xyz

Ruby: "ab" * 3
来源：http://fvt.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tzc.ctjpmb.com

[E03] 截取子串
来源：http://kxc.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://doe.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gle.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sot.fengsongda.top

TS:   s.slice(1, 4)
来源：http://huf.yfazqb.com

Java: s.substring(1, 4)
来源：http://osq.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cxz.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://uvn.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://ucd.52xcode.cn

[E04] 查找子串位置
来源：http://smm.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://eul.cucudq.cn

PHP:  strpos($s, "x");
来源：http://vca.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpa.uphjek.com

TS:   s.indexOf("x")
来源：http://wfe.fehbvm.com

Java: s.indexOf("x")
来源：http://agq.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://pdg.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://ams.aizwys.cn

C#:   s.IndexOf("x")
来源：http://rgn.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kfk.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gwh.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bcy.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqu.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://per.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyg.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rwn.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrj.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wir.gzhubu.top

[E06] 替换子串
来源：http://usp.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vfg.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://hew.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rhb.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://psv.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vwy.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pgs.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ltp.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://vgg.guowangkeji.top

[E07] 按分隔符拆分
来源：http://vow.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wxq.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zrx.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ump.guowangkeji.top

TS:   s.split(",")
来源：http://epv.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://mhh.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wdy.cashguo.top

Ruby: s.split(",");  s.split
来源：http://vko.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sih.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://ojt.hywenlv.cn

Py:   ",".join(items)
来源：http://jtk.sysykeji.top

PHP:  implode(",", $items);
来源：http://xim.xuetiantiany.cn

JS:   items.join(",")
来源：http://jeh.sufxvd.cn

TS:   items.join(",")
来源：http://lcx.yj20258.top

Java: String.join(",", items)
来源：http://whg.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://oja.hnqzz.top

Ruby: items.join(",")
来源：http://dgk.gotoacloud.top

C#:   string.Join(",", items)
来源：http://afk.svipenyu.cn

[E09] 去除所有空白字符
来源：http://yde.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gxl.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jwn.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://mes.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://gcj.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://nqh.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qxu.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qnc.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iur.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://iay.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jvw.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qdw.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://zln.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://wfr.ybcxt.top

Java: String.format("%03d", 7)
来源：http://swf.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://exz.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pmw.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uuu.tian-w.cn

[E11] 反转字符串
来源：http://dwx.pycfn.com

Py:   s[::-1]
来源：http://tbs.jyoumei.cn

PHP:  strrev($s);
来源：http://hwm.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://piv.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://wtn.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bsn.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hqj.xuetiantiany.cn

Ruby: s.reverse
来源：http://qod.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ntx.ydzc1.top

[E12] 统计某字符出现次数
来源：http://ybn.aizwys.cn

Py:   s.count("a")
来源：http://fkg.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://wfv.daxiang520.top

JS:   s.split("a").length - 1
来源：http://dmz.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://qqb.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eft.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://lio.vqdsnc.cn

Ruby: s.count("a")
来源：http://gna.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://cfg.jinqigufen.top

[E13] 逐字符遍历
来源：http://drb.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://bag.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jch.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uds.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gdw.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nyq.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://crq.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qle.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kqq.jianghu66.top

[E14] URL 编码与 Base64
来源：http://gfs.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xcx.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://sjf.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://emx.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ffp.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ehc.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsj.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rvg.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jrb.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://rjb.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://opp.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zev.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://boc.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rsk.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jwr.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yoq.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kna.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zvv.zhixingplan.top

[E16] 数字千分位
来源：http://oup.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://njj.tian-w.cn


<!-- 参考信息 -->