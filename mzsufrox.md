代发 wailian999

Java: list.size();
来源：http://fwb.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://pfb.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://wqr.quarkkingdee.top

C#:   list.Count;
来源：http://pqk.gzhubu.top

[D07] 切片 / 取子数组
来源：http://fnt.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hri.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wtc.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://dww.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://get.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://ruj.ydzc1.top

Go:   arr[1:4]
来源：http://vne.fengsongda.top

Ruby: arr[1, 3]
来源：http://lmf.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://vwt.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://cjh.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://lsa.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://yig.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bil.svipenyu.cn

TS:   [...a, ...b];
来源：http://zba.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dae.jyoumei.cn

Go:   append(a, b...)
来源：http://eox.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://itk.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://lng.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://tyw.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://ifu.yueranfly.top

PHP:  sort($arr);
来源：http://ogq.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oey.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ilq.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xjm.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qcv.sysykeji.top

Ruby: arr.sort
来源：http://opr.gaohongyu789.top

C#:   list.Sort();
来源：http://qnn.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://zcu.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yrm.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uor.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vvc.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nre.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvf.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipy.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zqf.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://agg.bjfxy.top

[D11] 反转数组
来源：http://dtq.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://niw.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://ylx.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eyk.yj20258.top

TS:   [...arr].reverse();
来源：http://lmr.hnqzz.top

Java: Collections.reverse(list);
来源：http://wbv.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://fcg.jqgufenzy.top

Ruby: arr.reverse
来源：http://yro.redwolf501.top

C#:   list.Reverse();
来源：http://txl.zhijiandao.cn

[D12] 查找元素下标
来源：http://zbu.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://pdo.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gjm.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ezu.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tmn.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxk.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://mmi.zycfv.cn

Ruby: arr.index(x)
来源：http://pie.fktsv.cn

C#:   list.IndexOf(x);
来源：http://mri.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://olm.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hou.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://arz.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://cyy.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://oof.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qrl.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://knb.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://icg.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ggh.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://nsd.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tfs.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://htt.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://jhd.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://ohl.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lnq.316326.xyz

Go:   // 手写循环
来源：http://zgj.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ecw.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jze.316326.xyz

[D15] 去重
来源：http://iwg.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bqm.jianghu66.top

PHP:  array_unique($arr);
来源：http://gos.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://sty.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://gvy.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lid.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ktv.hnqzz.top

Ruby: arr.uniq
来源：http://ena.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://idk.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://qvi.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qox.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmq.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yky.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://usk.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://btt.meibo888.top

Go:   // 手写循环累加
来源：http://kga.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iyz.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://abr.c1oappe.top

[D17] 最大值与最小值
来源：http://znm.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://vmg.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://azj.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lya.mhx1999.top

TS:   Math.max(...arr);
来源：http://ndr.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pkk.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wyy.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://klr.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://esw.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://miy.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sgd.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://cme.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rbj.hongshengwenyu.top

TS:   nested.flat();
来源：http://pqk.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://prm.gaohongyu789.top

Go:   // 手写双层循环
来源：http://wai.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://gsz.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nhm.jqgfzy.top

[D19] 按字段分组
来源：http://czi.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kwm.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kpt.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wbq.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://axr.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dnh.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://xxj.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nvq.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nlx.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://mzf.chenzaomai.com

Py:   Counter(arr)
来源：http://fju.sxryk.cn

PHP:  array_count_values($arr);
来源：http://bxd.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfv.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fyy.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iyf.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://vlo.zhijiandao.cn

Ruby: arr.tally
来源：http://zjf.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fqg.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://tou.svipenyu.cn

Py:   x in arr
来源：http://kdy.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://fwr.meibo888.top

JS:   arr.includes(x)
来源：http://vzv.redwolf501.top

TS:   arr.includes(x)
来源：http://cgy.ppjwa.cn

Java: list.contains(x)
来源：http://rip.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://fhs.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://ibp.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://atb.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://upv.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ily.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ffc.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rbe.fengsongda.top

TS:   [...arr];
来源：http://gzk.yj202588.top

Java: new ArrayList<>(list);
来源：http://ckc.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://qim.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://jiy.jinqigfzy.top

C#:   new List<int>(list);
来源：http://ugk.zhijiandao.cn

[D23] reduce 累积计算
来源：http://qox.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://shm.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rwc.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vtt.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zww.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://wzr.yongpay.top

Go:   // 手写循环
来源：http://dwz.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mmm.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctc.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://raa.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ody.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wzj.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://epf.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wop.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xrr.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ovy.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rdd.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dlr.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://sct.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yhk.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xae.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xxh.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgg.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ahu.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pom.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lli.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rgc.xinyue.icu

[D26] 数组转字符串
来源：http://scw.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://mwc.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://nme.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://jwn.xuanzx.com

TS:   arr.join(", ")
来源：http://mwa.fengsongda.top

Java: String.join(", ", list)
来源：http://ibj.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://raq.yj20258.top

Ruby: arr.join(", ")
来源：http://mzt.bjfxy.top

C#:   string.Join(", ", list)
来源：http://ryo.yuxming.cn

================================================================================
来源：http://fov.bbcook.cn

E. 字符串处理
来源：http://jfa.fzhhl.top

================================================================================
来源：http://cer.zdqjudy.top

[E01] 拼接字符串
来源：http://qbg.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owk.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aol.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hiy.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ghw.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://klj.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mjr.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zmd.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yrd.ppjwa.cn

[E02] 重复字符串
来源：http://kig.ydzc1.top

Py:   "ab" * 3
来源：http://unn.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://bbg.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://thz.mhx1999.top

TS:   "ab".repeat(3)
来源：http://fcz.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://jpk.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://cex.tanke756.top

Ruby: "ab" * 3
来源：http://pzm.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xtr.ydjk.org.cn

[E03] 截取子串
来源：http://cma.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xtf.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://boi.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hus.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://ybi.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://vna.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jrm.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://xgl.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://qck.dianchejie.cn

[E04] 查找子串位置
来源：http://awh.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://tvr.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://oiy.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yrs.cucudq.cn

TS:   s.indexOf("x")
来源：http://nfy.cdnleiting.top

Java: s.indexOf("x")
来源：http://lzr.yj202588.top

Go:   strings.Index(s, "x")
来源：http://dux.bjfxy.top

Ruby: s.index("x")
来源：http://jjz.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://swk.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jde.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uqe.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qva.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://srf.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jyd.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pfk.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://buc.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wdp.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zoa.tarul.cn

[E06] 替换子串
来源：http://zks.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dxn.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://ztd.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://byk.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://fsp.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ihw.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tqi.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://twz.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://plj.shuidangran.top

[E07] 按分隔符拆分
来源：http://bab.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bji.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://duu.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mwf.jyoumei.cn

TS:   s.split(",")
来源：http://zzt.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jsy.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fsn.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://szy.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gxl.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://zen.epnwcf.com

Py:   ",".join(items)
来源：http://haw.nanxinkj.top

PHP:  implode(",", $items);
来源：http://tcp.52xcode.cn

JS:   items.join(",")
来源：http://uoi.aizwys.cn

TS:   items.join(",")
来源：http://rja.hysaishi.cn

Java: String.join(",", items)
来源：http://jiw.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://yjc.tarul.cn

Ruby: items.join(",")
来源：http://odc.jyoumei.cn

C#:   string.Join(",", items)
来源：http://vkb.zhixingplan.top

[E09] 去除所有空白字符
来源：http://ayo.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aaq.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xkl.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://rrx.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://qbh.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ufm.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vdz.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kgx.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aik.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://src.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gpr.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cvb.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://dfc.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://gur.yuxming.cn

Java: String.format("%03d", 7)
来源：http://luj.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://arv.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ths.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jsk.cucudq.cn

[E11] 反转字符串
来源：http://jib.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://zbb.ctjpmb.com

PHP:  strrev($s);
来源：http://etq.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://ovj.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://zjr.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zbq.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://djp.hywenlv.cn

Ruby: s.reverse
来源：http://ses.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kwt.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://rsq.iojbl.cn

Py:   s.count("a")
来源：http://qzq.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://uvf.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://jmi.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://wji.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gtx.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://ehn.jqgfzy.top

Ruby: s.count("a")
来源：http://cga.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://ojq.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://jzj.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://ymx.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://asg.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://olr.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ela.zhijiandao.cn


<!-- 参考信息 -->