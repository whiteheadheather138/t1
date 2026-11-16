代发 wailian999

TS:   arr.slice(1, 4);
来源：http://bft.xziqi.cn

Java: list.subList(1, 4);
来源：http://eip.sxryk.cn

Go:   arr[1:4]
来源：http://gox.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://uvt.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://jrx.gzhubu.top

[D08] 合并两个数组
来源：http://rri.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://aud.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://yen.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://esk.ybcxt.top

TS:   [...a, ...b];
来源：http://inw.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pjr.tanke756.top

Go:   append(a, b...)
来源：http://ouo.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://vnd.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://bea.bjfxy.top

[D09] 排序（升序）
来源：http://eit.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://awx.chenzaomai.com

PHP:  sort($arr);
来源：http://eae.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kup.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfz.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nyi.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jqi.yfazqb.com

Ruby: arr.sort
来源：http://mcd.chenjidiqi.icu

C#:   list.Sort();
来源：http://zli.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nok.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dza.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tds.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tzr.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ljk.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vgx.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://brb.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://siq.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fgl.svipenyu.cn

[D11] 反转数组
来源：http://lfe.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://twp.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://vnl.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ofg.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://nuv.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://ehc.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://gmd.pycfn.com

Ruby: arr.reverse
来源：http://iql.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://zat.wangdashe.top

[D12] 查找元素下标
来源：http://sfk.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://gnv.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ubi.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrb.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbs.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dze.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://dvu.gotoacloud.top

Ruby: arr.index(x)
来源：http://ofw.smart0.xyz

C#:   list.IndexOf(x);
来源：http://pgi.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://eht.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://chz.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://krv.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://xsq.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://fnj.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ezv.shangyingyoupin.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rra.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://aps.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tyj.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://cwk.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kyp.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ces.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://ukh.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://akp.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfw.daria6918.cn

Go:   // 手写循环
来源：http://mhw.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://rrq.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://zgz.daria6918.cn

[D15] 去重
来源：http://vll.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vll.c1oappe.top

PHP:  array_unique($arr);
来源：http://kuv.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://oxs.sxryk.cn

TS:   [...new Set(arr)]
来源：http://kgs.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lvd.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://ogz.hcnkem.com

Ruby: arr.uniq
来源：http://htr.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://pll.wangshuangyany.cn

[D16] 求和与平均值
来源：http://fpd.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsb.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ucy.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajm.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qdc.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lms.hammf.cn

Go:   // 手写循环累加
来源：http://dky.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nnw.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://qud.52xcode.cn

[D17] 最大值与最小值
来源：http://qol.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://adn.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://wml.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lbb.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://eky.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wlm.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://etc.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://icc.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://quj.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://kaq.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://reg.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://prg.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nln.vehdjk.com

TS:   nested.flat();
来源：http://rmq.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uoo.dashuyun.cn

Go:   // 手写双层循环
来源：http://ddv.xziqi.cn

Ruby: nested.flatten
来源：http://ram.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tun.gotoacloud.top

[D19] 按字段分组
来源：http://jkw.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mno.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mzw.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afh.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ndu.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ihu.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://lyy.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mwx.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbc.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://rmz.hesvh.cn

Py:   Counter(arr)
来源：http://ymv.cheryme.top

PHP:  array_count_values($arr);
来源：http://lpb.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zuy.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vhd.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kpa.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://cmk.hcnkem.com

Ruby: arr.tally
来源：http://loi.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qan.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://xzh.jqgfzy.top

Py:   x in arr
来源：http://dvs.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://wje.jlsjyb.cn

JS:   arr.includes(x)
来源：http://pyf.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://dbw.bjfxy.top

Java: list.contains(x)
来源：http://lyr.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://aaa.xinyue.icu

Ruby: arr.include?(x)
来源：http://qgo.hfpthk.cn

C#:   list.Contains(x)
来源：http://oic.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://rec.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lqu.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://asf.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zva.zhijiandao.cn

TS:   [...arr];
来源：http://vur.birdmap.top

Java: new ArrayList<>(list);
来源：http://lsx.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://ejh.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://qhj.yuxming.cn

C#:   new List<int>(list);
来源：http://lru.xziqi.cn

[D23] reduce 累积计算
来源：http://fde.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://egm.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vsp.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ret.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ibt.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hbl.52xcode.cn

Go:   // 手写循环
来源：http://gub.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fxn.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kei.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://fiz.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oqc.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lfq.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qhu.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qjv.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kqp.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ixa.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cnp.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mbl.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://vch.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bkb.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dku.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lfj.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hgz.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jjy.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yjw.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qxb.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ycn.shangyingyoupin.top

[D26] 数组转字符串
来源：http://zqh.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://ont.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://fbf.nanxuanxn.top

JS:   arr.join(", ")
来源：http://ggx.cheryme.top

TS:   arr.join(", ")
来源：http://gpe.gzhubu.top

Java: String.join(", ", list)
来源：http://dpj.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://uin.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://qok.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://itj.jiagoushi.top

================================================================================
来源：http://vux.fengsongda.top

E. 字符串处理
来源：http://ojf.vehdjk.com

================================================================================
来源：http://gcv.jyoumei.cn

[E01] 拼接字符串
来源：http://efv.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qtu.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kxt.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ret.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwh.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xqd.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bwj.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xrm.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vnb.sufxvd.cn

[E02] 重复字符串
来源：http://dzb.9152youxi.cn

Py:   "ab" * 3
来源：http://fua.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://adx.xylfe.cn

JS:   "ab".repeat(3)
来源：http://hpq.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://ggp.52xcode.cn

Java: "ab".repeat(3)
来源：http://iry.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://luc.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://jvc.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://epy.ydjk.org.cn

[E03] 截取子串
来源：http://iik.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://chw.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fbo.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mbt.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://uvj.xuanzx.com

Java: s.substring(1, 4)
来源：http://pfv.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gmw.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://eqi.yj202588.top

C#:   s.Substring(1, 3)
来源：http://iac.ppjwa.cn

[E04] 查找子串位置
来源：http://bnp.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://csg.fehbvm.com

PHP:  strpos($s, "x");
来源：http://lxz.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqr.uphjek.com

TS:   s.indexOf("x")
来源：http://qnd.ybcxt.top

Java: s.indexOf("x")
来源：http://car.yj202588.top

Go:   strings.Index(s, "x")
来源：http://fst.sufxvd.cn

Ruby: s.index("x")
来源：http://jsj.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://scd.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gbt.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zng.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wfw.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxe.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvy.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuu.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hjm.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ien.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vwc.sjlbkw.cn

[E06] 替换子串
来源：http://rlh.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ifq.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://vgl.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kxn.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://uwr.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cre.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://piw.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://red.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://ygk.xziqi.cn

[E07] 按分隔符拆分
来源：http://kyg.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lnm.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fce.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ppy.zhengqikj.top

TS:   s.split(",")
来源：http://isg.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fum.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://snk.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://lec.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vaj.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://amv.ppjwa.cn

Py:   ",".join(items)
来源：http://crb.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://lkn.nwbrower.top

JS:   items.join(",")
来源：http://ycz.ivvv.top

TS:   items.join(",")
来源：http://scp.quarkkingdee.top

Java: String.join(",", items)
来源：http://gwi.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://mdc.jlsjyb.cn

Ruby: items.join(",")
来源：http://wqc.cashguo.top

C#:   string.Join(",", items)
来源：http://dgh.gzhubu.top

[E09] 去除所有空白字符
来源：http://xdr.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ojq.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tpc.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://lft.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://tau.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://wiu.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eau.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://mhh.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cot.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://isu.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cle.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qwi.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://dyh.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://tzi.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://aow.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vte.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fvm.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://agp.pengpengdd.cyou

[E11] 反转字符串
来源：http://tcu.xziqi.cn

Py:   s[::-1]
来源：http://jwp.xziqi.cn

PHP:  strrev($s);
来源：http://rzd.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://mng.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://uub.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tjh.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tbx.xuanzx.com

Ruby: s.reverse
来源：http://zxr.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://jmg.guannengcc.top

[E12] 统计某字符出现次数
来源：http://nvk.yuanzhike.top

Py:   s.count("a")
来源：http://snf.meibo888.top

PHP:  substr_count($s, "a");
来源：http://mnq.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://hza.hnqzz.top

TS:   s.split("a").length - 1
来源：http://tux.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://twu.gogol.net.cn

Go:   strings.Count(s, "a")
来源：http://wko.xuetiantiany.cn

Ruby: s.count("a")
来源：http://hxp.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://vzh.birdmap.top

[E13] 逐字符遍历
来源：http://tcr.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://adt.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xfj.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://wdd.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qgl.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yhx.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mwg.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://wsw.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bwe.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://qhf.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ocf.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cxw.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zvl.jiagoushi.top


<!-- 参考信息 -->