代发 wailian999

Java: list.size();
来源：http://yjy.pengpengdd.cyou

Go:   len(arr)
来源：http://dsl.sysykeji.top

Ruby: arr.length; arr.size
来源：http://jwj.zdbjq.cn

C#:   list.Count;
来源：http://fbl.ydzc1.top

[D07] 切片 / 取子数组
来源：http://xrk.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lxm.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://euq.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://zmb.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://ddn.316326.xyz

Java: list.subList(1, 4);
来源：http://zuy.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://zxd.316326.xyz

Ruby: arr[1, 3]
来源：http://vha.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://oxg.zdqjudy.top

[D08] 合并两个数组
来源：http://gvi.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://upm.yonumen.top

PHP:  array_merge($a, $b);
来源：http://bqw.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ppg.tian-w.cn

TS:   [...a, ...b];
来源：http://agu.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://apw.hcnkem.com

Go:   append(a, b...)
来源：http://lma.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://sjo.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://zwp.vqdsnc.cn

[D09] 排序（升序）
来源：http://ubq.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://wwn.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://aoz.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hoq.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://apo.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ldp.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hly.bjfxy.top

Ruby: arr.sort
来源：http://cms.zhijiandao.cn

C#:   list.Sort();
来源：http://ovw.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wqo.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wxs.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwc.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://csv.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hrp.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gtw.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://otf.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ujb.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxa.wangdashe.top

[D11] 反转数组
来源：http://ceu.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://pin.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://fds.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rhc.fzhhl.top

TS:   [...arr].reverse();
来源：http://daa.ehwqpu.com

Java: Collections.reverse(list);
来源：http://btf.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://xeb.sufxvd.cn

Ruby: arr.reverse
来源：http://akx.hesvh.cn

C#:   list.Reverse();
来源：http://qac.hysaishi.cn

[D12] 查找元素下标
来源：http://twm.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://dri.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cqz.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fed.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcg.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aai.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://tso.316326.xyz

Ruby: arr.index(x)
来源：http://rnw.guannengcc.top

C#:   list.IndexOf(x);
来源：http://jtw.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://zjj.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jfb.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hwg.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://xcc.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://gtp.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xhu.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mez.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://awu.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hxb.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://utj.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jfp.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ccc.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://huj.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://ehe.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://enm.shuidangran.top

Go:   // 手写循环
来源：http://fuv.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://luj.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://muv.shangyingyoupin.top

[D15] 去重
来源：http://wzr.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vuk.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://mnl.tanke756.top

JS:   [...new Set(arr)]
来源：http://nwh.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://qab.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hbw.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://emt.yj202588.top

Ruby: arr.uniq
来源：http://qph.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://iep.fktsv.cn

[D16] 求和与平均值
来源：http://laa.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nip.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fux.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mey.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zni.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://weg.zhongyouzk.top

Go:   // 手写循环累加
来源：http://euc.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://etr.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://gnb.zdqjudy.top

[D17] 最大值与最小值
来源：http://cnc.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://yvx.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://eoz.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qhx.dianchejie.cn

TS:   Math.max(...arr);
来源：http://icx.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://pdr.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vsz.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://fis.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://avf.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://qfw.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wst.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://pzt.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qej.wangdashe.top

TS:   nested.flat();
来源：http://bxy.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rwn.316326.xyz

Go:   // 手写双层循环
来源：http://zbk.iojbl.cn

Ruby: nested.flatten
来源：http://lhf.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tnj.zhixingplan.top

[D19] 按字段分组
来源：http://jau.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gpg.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zzd.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ccf.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://smv.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uwr.birdmap.top

Go:   // 手写 map[string][]T
来源：http://qxa.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ivl.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eju.yj20258.top

[D20] 统计每个元素出现次数
来源：http://crh.feifeiyinyue.top

Py:   Counter(arr)
来源：http://nbg.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://zcf.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mxo.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ncw.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ine.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://vrq.mhx1999.top

Ruby: arr.tally
来源：http://sev.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swt.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://hwa.yj20258888.top

Py:   x in arr
来源：http://dlc.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://nht.xinyue.icu

JS:   arr.includes(x)
来源：http://cgx.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://opz.dashuyun.cn

Java: list.contains(x)
来源：http://evq.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://yls.hnqzz.top

Ruby: arr.include?(x)
来源：http://ylu.guannengcc.top

C#:   list.Contains(x)
来源：http://fki.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://nfm.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://obw.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://azr.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://amd.zhixingplan.top

TS:   [...arr];
来源：http://xet.tanke756.top

Java: new ArrayList<>(list);
来源：http://xyx.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://nyp.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://trj.hcnkem.com

C#:   new List<int>(list);
来源：http://ono.bjfxy.top

[D23] reduce 累积计算
来源：http://paa.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jpv.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hbw.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgi.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tge.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://csd.hesvh.cn

Go:   // 手写循环
来源：http://kug.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://owo.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uny.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://nyv.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjr.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vzy.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ftq.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jjp.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtp.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ytu.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esj.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dif.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://pcr.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zzl.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://idx.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fkf.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://enf.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://opj.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hyq.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lqg.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pcu.pengpengdd.cyou

[D26] 数组转字符串
来源：http://tse.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://ahc.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://isu.gotoacloud.top

JS:   arr.join(", ")
来源：http://gwv.cucudq.cn

TS:   arr.join(", ")
来源：http://wmi.zhijiandao.cn

Java: String.join(", ", list)
来源：http://odm.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://lma.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://xif.aizwys.cn

C#:   string.Join(", ", list)
来源：http://jzk.quarkkingdee.top

================================================================================
来源：http://skp.jyoumei.cn

E. 字符串处理
来源：http://lfh.zdbjq.cn

================================================================================
来源：http://pkc.nanxuanxn.top

[E01] 拼接字符串
来源：http://owe.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jvi.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nsu.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nsq.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dri.guannengcc.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vrq.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zlh.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xhc.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sgj.52xcode.cn

[E02] 重复字符串
来源：http://jea.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://qit.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://xjl.sysykeji.top

JS:   "ab".repeat(3)
来源：http://uzb.jianghu66.top

TS:   "ab".repeat(3)
来源：http://ove.yj20258.top

Java: "ab".repeat(3)
来源：http://lfe.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://mbu.zhijiandao.cn

Ruby: "ab" * 3
来源：http://yhm.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fbz.pengpengdd.cyou

[E03] 截取子串
来源：http://yka.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tir.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zje.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ndl.ybcxt.top

TS:   s.slice(1, 4)
来源：http://ttf.yfazqb.com

Java: s.substring(1, 4)
来源：http://vlv.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://exx.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://nzn.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://jcx.guannengcc.top

[E04] 查找子串位置
来源：http://upc.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://mkj.pycfn.com

PHP:  strpos($s, "x");
来源：http://quv.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qxh.nanxinkj.top

TS:   s.indexOf("x")
来源：http://epg.ppjwa.cn

Java: s.indexOf("x")
来源：http://qlb.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://ixm.shangyingyoupin.top

Ruby: s.index("x")
来源：http://ngr.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://cyk.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijm.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jrn.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lty.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qwk.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nhk.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrt.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wil.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njg.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dmt.fanxiaobao.xyz

[E06] 替换子串
来源：http://pdk.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sic.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://gpi.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://azw.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://tce.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wos.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ycx.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ori.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://dkq.fzhhl.top

[E07] 按分隔符拆分
来源：http://xer.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mdl.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jnh.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nqm.0kj1m.cn

TS:   s.split(",")
来源：http://wdp.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://rjt.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kbg.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://qzv.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tam.uphjek.com

[E08] 数组按分隔符合并
来源：http://bvl.jianghu66.top

Py:   ",".join(items)
来源：http://kzh.yfazqb.com

PHP:  implode(",", $items);
来源：http://hgw.xziqi.cn

JS:   items.join(",")
来源：http://yzw.epnwcf.com

TS:   items.join(",")
来源：http://vcp.aibaodan.cn

Java: String.join(",", items)
来源：http://dyu.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://bva.jinqigfzy.top

Ruby: items.join(",")
来源：http://zvj.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://raw.hfpthk.cn

[E09] 去除所有空白字符
来源：http://fjf.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://osy.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://svw.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://kuw.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://jvp.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://ayi.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vvw.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://xnf.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hwp.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://cpi.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lpw.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vju.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://ggr.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://yvn.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://njb.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ejf.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gic.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nus.hcnkem.com

[E11] 反转字符串
来源：http://sll.hesvh.cn

Py:   s[::-1]
来源：http://slo.aibaodan.cn

PHP:  strrev($s);
来源：http://gic.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://dji.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://svj.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://efs.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fjx.yongpay.top

Ruby: s.reverse
来源：http://loh.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://vau.andypj.xyz

[E12] 统计某字符出现次数
来源：http://mkn.epnwcf.com

Py:   s.count("a")
来源：http://ctr.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://wsi.cheryme.top

JS:   s.split("a").length - 1
来源：http://cql.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://asm.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sem.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://bkm.dashuyun.cn

Ruby: s.count("a")
来源：http://fmy.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://sqg.yj202588.top

[E13] 逐字符遍历
来源：http://xpo.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://qka.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jry.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vbk.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yiv.nanxinkj.top


<!-- 参考信息 -->