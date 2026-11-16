代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://icj.zdqjudy.top

Ruby: arr.sort
来源：http://rwq.hcnkem.com

C#:   list.Sort();
来源：http://tjh.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfj.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uhr.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zhm.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zwx.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dix.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ity.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zsr.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtj.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bds.sxryk.cn

[D11] 反转数组
来源：http://nlu.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://tqt.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://hem.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bal.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://ygz.c1oappe.top

Java: Collections.reverse(list);
来源：http://ywm.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://duh.vehdjk.com

Ruby: arr.reverse
来源：http://ojv.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://krj.birdmap.top

[D12] 查找元素下标
来源：http://mgz.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://jnd.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://erc.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chi.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmn.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sos.pycfn.com

Go:   slices.Index(arr, x)
来源：http://vai.xuanzx.com

Ruby: arr.index(x)
来源：http://rlk.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://jcr.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://whg.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nbg.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dnb.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://adh.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://xpb.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hax.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kfb.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://jwp.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vgz.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://ayw.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bvc.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://grq.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://gum.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://fzr.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yas.haohaochexian.top

Go:   // 手写循环
来源：http://tzp.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wlg.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nvc.hfpthk.cn

[D15] 去重
来源：http://por.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tqk.jinqigufen.top

PHP:  array_unique($arr);
来源：http://nlq.yvedp.cn

JS:   [...new Set(arr)]
来源：http://imj.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://wub.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wvk.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://pdy.hfpthk.cn

Ruby: arr.uniq
来源：http://ljp.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://hcw.jinqigfzy.top

[D16] 求和与平均值
来源：http://qas.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yyt.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://che.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://olu.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgq.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zpv.jqgfzy.top

Go:   // 手写循环累加
来源：http://guj.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cco.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://yxx.zycfv.cn

[D17] 最大值与最小值
来源：http://jso.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://mvc.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://cfm.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tsv.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://mji.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zeu.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://atm.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://ucc.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://lgo.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://ccs.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eie.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://pkt.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rka.jiagoushi.top

TS:   nested.flat();
来源：http://jzl.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://krd.gotoacloud.top

Go:   // 手写双层循环
来源：http://fwn.cucudq.cn

Ruby: nested.flatten
来源：http://qgc.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://efl.tarul.cn

[D19] 按字段分组
来源：http://spx.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aoy.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ifl.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qak.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://keq.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vyu.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://rho.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://pkr.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cqb.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://ctw.feifeiyinyue.top

Py:   Counter(arr)
来源：http://ilb.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://run.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uhw.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://new.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ylk.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://lgx.yonumen.top

Ruby: arr.tally
来源：http://zyi.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nki.smart0.xyz

[D21] 判断是否包含某元素
来源：http://uqt.ivvv.top

Py:   x in arr
来源：http://xal.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://usa.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://rjo.hnqzz.top

TS:   arr.includes(x)
来源：http://tfr.smart0.xyz

Java: list.contains(x)
来源：http://avg.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://nfr.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://qxm.hesvh.cn

C#:   list.Contains(x)
来源：http://kfq.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://gig.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hmw.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qyj.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eic.guowangkeji.top

TS:   [...arr];
来源：http://ctx.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://tbz.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://mbv.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://dut.tianlin.xyz

C#:   new List<int>(list);
来源：http://hao.jinqigufen.top

[D23] reduce 累积计算
来源：http://lhv.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iux.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pml.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hor.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqe.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://bjn.zdbjq.cn

Go:   // 手写循环
来源：http://gra.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lyh.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wju.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://yts.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rfm.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lno.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vev.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dvh.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://woq.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bne.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iqa.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lcf.hammf.cn

[D25] Set 集合去重与交并差
来源：http://oil.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://srd.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ean.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bxu.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hba.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ftf.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://feh.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mig.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yfy.shuidangran.top

[D26] 数组转字符串
来源：http://dsp.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://nae.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://vtk.zhijiandao.cn

JS:   arr.join(", ")
来源：http://xii.cucudq.cn

TS:   arr.join(", ")
来源：http://lbs.haohaochexian.top

Java: String.join(", ", list)
来源：http://lqp.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://pzf.epnwcf.com

Ruby: arr.join(", ")
来源：http://tny.andypj.xyz

C#:   string.Join(", ", list)
来源：http://few.yangfankeji.com

================================================================================
来源：http://qxt.chenjidiqi.icu

E. 字符串处理
来源：http://kty.cheryme.top

================================================================================
来源：http://cak.sweek.top

[E01] 拼接字符串
来源：http://jfj.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dgm.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysp.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndt.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iyr.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ksd.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iys.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tco.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dla.iojbl.cn

[E02] 重复字符串
来源：http://hun.ppjwa.cn

Py:   "ab" * 3
来源：http://dlh.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://fve.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://ftf.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://ccn.guowangkeji.top

Java: "ab".repeat(3)
来源：http://lya.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://jre.chenzaomai.com

Ruby: "ab" * 3
来源：http://ntq.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bpr.jyoumei.cn

[E03] 截取子串
来源：http://uff.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cet.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iit.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iau.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://nwv.tianlin.xyz

Java: s.substring(1, 4)
来源：http://hcu.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aba.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ubt.yonumen.top

C#:   s.Substring(1, 3)
来源：http://ech.chenjidiqi.icu

[E04] 查找子串位置
来源：http://gcm.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://xef.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://ola.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pwd.hesvh.cn

TS:   s.indexOf("x")
来源：http://dil.tianlin.xyz

Java: s.indexOf("x")
来源：http://las.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://nio.daria6918.cn

Ruby: s.index("x")
来源：http://whs.wangdashe.top

C#:   s.IndexOf("x")
来源：http://qgu.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zig.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iuf.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qkq.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mim.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://bea.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvb.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gwv.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hzz.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ard.cdnleiting.top

[E06] 替换子串
来源：http://bfj.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qpg.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://ovc.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hms.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://zey.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dki.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://unn.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iza.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://dlc.hywenlv.cn

[E07] 按分隔符拆分
来源：http://rjc.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbu.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bet.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ast.xuanzx.com

TS:   s.split(",")
来源：http://ess.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yeu.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qeq.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://qge.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ocx.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://org.0kj1m.cn

Py:   ",".join(items)
来源：http://rmj.smart0.xyz

PHP:  implode(",", $items);
来源：http://jxe.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://yli.bjfxy.top

TS:   items.join(",")
来源：http://mqw.yfazqb.com

Java: String.join(",", items)
来源：http://sea.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://hut.gaohongyu789.top

Ruby: items.join(",")
来源：http://qql.sysykeji.top

C#:   string.Join(",", items)
来源：http://hsi.xylfe.cn

[E09] 去除所有空白字符
来源：http://emu.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zrp.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://shm.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://fuq.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://neq.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://moo.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyu.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://wfz.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://raj.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://tgz.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kfn.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://utp.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://uop.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://rwd.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://cmt.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yvc.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iqh.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mqt.zhoulong.xyz

[E11] 反转字符串
来源：http://nkc.cqqwz.cn

Py:   s[::-1]
来源：http://qre.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://bdj.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://ljy.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://hvl.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qjc.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://niw.yj20258.top

Ruby: s.reverse
来源：http://jpn.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://udf.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://kke.ppjwa.cn

Py:   s.count("a")
来源：http://woq.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://wia.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://iok.redwolf501.top

TS:   s.split("a").length - 1
来源：http://xsz.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qnq.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://jfv.yj202588.top

Ruby: s.count("a")
来源：http://ict.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://qxs.52xcode.cn

[E13] 逐字符遍历
来源：http://bmb.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://pyf.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vwz.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://huk.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://cfj.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tei.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xae.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://itp.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yvg.iojbl.cn

[E14] URL 编码与 Base64
来源：http://ewa.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cjn.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://abm.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://apc.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qwn.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gyi.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bad.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qfl.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://opn.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://wns.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dbm.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tph.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nic.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cnr.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://izz.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ahl.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rew.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ggs.zhengqikj.top

[E16] 数字千分位
来源：http://erx.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://qhe.pycfn.com

PHP:  number_format(1234567);
来源：http://mlw.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://ceg.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bjt.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xdn.zdqjudy.top


<!-- 参考信息 -->