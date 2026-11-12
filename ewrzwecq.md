代发 wailian999

TS:   arr.slice(1, 4);
来源：http://thl.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://mln.yuanzhike.top

Go:   arr[1:4]
来源：http://riy.birdmap.top

Ruby: arr[1, 3]
来源：http://tmy.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://eiy.jianghu66.top

[D08] 合并两个数组
来源：http://lqw.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://aqz.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://ehs.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aij.gzhubu.top

TS:   [...a, ...b];
来源：http://usj.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dxk.aibaodan.cn

Go:   append(a, b...)
来源：http://cgb.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://daw.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://iaj.zhoulong.xyz

[D09] 排序（升序）
来源：http://yhr.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qni.zhoulong.xyz

PHP:  sort($arr);
来源：http://yhu.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hja.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://ead.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ifv.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rie.yuanzhike.top

Ruby: arr.sort
来源：http://mui.wangshuangyany.cn

C#:   list.Sort();
来源：http://vws.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jpg.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://szt.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://loi.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pmz.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvz.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xsq.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cjz.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nyf.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jqv.c1oappe.top

[D11] 反转数组
来源：http://adn.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://kgi.fzhhl.top

PHP:  array_reverse($arr);
来源：http://cdm.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://igd.yongpay.top

TS:   [...arr].reverse();
来源：http://ikr.andypj.xyz

Java: Collections.reverse(list);
来源：http://euu.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://fpl.tian-w.cn

Ruby: arr.reverse
来源：http://lba.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://kxi.guowangkeji.top

[D12] 查找元素下标
来源：http://icm.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://zrz.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://szq.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://abh.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfp.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nmi.316326.xyz

Go:   slices.Index(arr, x)
来源：http://ibj.xylfe.cn

Ruby: arr.index(x)
来源：http://lwc.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://rga.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://ptb.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fgy.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://feq.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://oga.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://irk.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yah.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bdo.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zyi.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fpo.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://qpt.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jru.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yry.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://yil.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://cxu.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ged.fehbvm.com

Go:   // 手写循环
来源：http://whh.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://ozh.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tpq.yfazqb.com

[D15] 去重
来源：http://pdv.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oyd.tarul.cn

PHP:  array_unique($arr);
来源：http://jqk.bbcook.cn

JS:   [...new Set(arr)]
来源：http://epr.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://bby.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bla.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://iwe.jyoumei.cn

Ruby: arr.uniq
来源：http://jgn.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://aoq.hesvh.cn

[D16] 求和与平均值
来源：http://rvb.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wrf.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eip.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrc.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yov.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jix.shuidangran.top

Go:   // 手写循环累加
来源：http://ugc.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zjs.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://jfq.fengsongda.top

[D17] 最大值与最小值
来源：http://eav.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://ysr.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://cnj.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xgl.zhixingplan.top

TS:   Math.max(...arr);
来源：http://lar.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://nul.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rad.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://ahz.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://zpe.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://uid.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vwe.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://weg.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lev.birdmap.top

TS:   nested.flat();
来源：http://sdg.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://scy.aibaodan.cn

Go:   // 手写双层循环
来源：http://sls.birdmap.top

Ruby: nested.flatten
来源：http://smi.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tpf.jiagoushi.top

[D19] 按字段分组
来源：http://yps.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iai.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ocu.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://agn.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yuc.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kou.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://wmx.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cub.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ftp.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://fdv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://fay.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://tts.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nqf.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gfk.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ssd.cheryme.top

Go:   // 手写 map[T]int
来源：http://sxq.hysaishi.cn

Ruby: arr.tally
来源：http://snl.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vmu.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://gam.yangfankeji.com

Py:   x in arr
来源：http://zuc.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://sjm.gotoacloud.top

JS:   arr.includes(x)
来源：http://xtp.yvedp.cn

TS:   arr.includes(x)
来源：http://pgn.nwbrower.top

Java: list.contains(x)
来源：http://zss.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://lfi.yvedp.cn

Ruby: arr.include?(x)
来源：http://pnd.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://igf.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://qor.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jtr.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sol.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://smg.sxryk.cn

TS:   [...arr];
来源：http://ucc.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://fww.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://veu.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://llo.yj20258.top

C#:   new List<int>(list);
来源：http://net.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://nqc.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://asf.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oez.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyx.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpw.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fpz.tarul.cn

Go:   // 手写循环
来源：http://clx.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bbe.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hcr.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://krj.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rbb.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wag.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zeu.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lwt.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dqe.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fjw.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nlx.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://irs.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://pyf.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cto.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vxu.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rql.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zii.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ndr.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ift.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nje.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sww.bbcook.cn

[D26] 数组转字符串
来源：http://inz.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://eus.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://nxi.jinqigufen.top

JS:   arr.join(", ")
来源：http://dcd.ydjk.org.cn

TS:   arr.join(", ")
来源：http://mzz.aibaodan.cn

Java: String.join(", ", list)
来源：http://ykm.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://bbl.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://euv.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://dpp.shzxlz.cn

================================================================================
来源：http://aut.cdnleiting.top

E. 字符串处理
来源：http://sdl.xylfe.cn

================================================================================
来源：http://paj.zhijiandao.cn

[E01] 拼接字符串
来源：http://enm.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://upq.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcv.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyp.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zna.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pqv.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rrg.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axt.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jtg.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://wbf.sjlbkw.cn

Py:   "ab" * 3
来源：http://lqh.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://zrw.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://zvl.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://muk.dashuyun.cn

Java: "ab".repeat(3)
来源：http://fqv.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://isi.sjlbkw.cn

Ruby: "ab" * 3
来源：http://isf.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lby.kuanghao11.cn

[E03] 截取子串
来源：http://lrk.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uam.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dos.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ftm.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://tjd.shzxlz.cn

Java: s.substring(1, 4)
来源：http://cqz.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lbl.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://egm.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://org.yvedp.cn

[E04] 查找子串位置
来源：http://stj.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://smf.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://ulq.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tbo.epnwcf.com

TS:   s.indexOf("x")
来源：http://gwo.52xcode.cn

Java: s.indexOf("x")
来源：http://wqs.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://bsq.yuxming.cn

Ruby: s.index("x")
来源：http://isd.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://jdi.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://yvc.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qab.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rfu.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfl.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gmq.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bml.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mky.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hgg.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hqz.sxryk.cn

[E06] 替换子串
来源：http://yap.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zrh.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://nuq.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rjv.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://kda.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xbl.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rqy.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pch.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://xwx.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://giu.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://acq.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xdn.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ngb.zhixingplan.top

TS:   s.split(",")
来源：http://qoy.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cth.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iio.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://piy.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ica.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://bbc.vehdjk.com

Py:   ",".join(items)
来源：http://doz.gzhubu.top

PHP:  implode(",", $items);
来源：http://ggg.ybcxt.top

JS:   items.join(",")
来源：http://ces.pycfn.com

TS:   items.join(",")
来源：http://ydr.yangfankeji.com

Java: String.join(",", items)
来源：http://sfn.yonumen.top

Go:   strings.Join(items, ",")
来源：http://oei.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://now.iojbl.cn

C#:   string.Join(",", items)
来源：http://uno.yfazqb.com

[E09] 去除所有空白字符
来源：http://tkw.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hkg.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ruk.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://qut.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://bis.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://rwu.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://bjx.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://fnl.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://afn.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://mkg.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kdv.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jbd.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://pem.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://bzv.hnqzz.top

Java: String.format("%03d", 7)
来源：http://xba.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://tcq.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tpv.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gto.kuanghao11.cn

[E11] 反转字符串
来源：http://zzo.gotoacloud.top

Py:   s[::-1]
来源：http://ttc.yangfankeji.com

PHP:  strrev($s);
来源：http://qsy.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://rvi.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://jca.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://waf.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ksg.epnwcf.com

Ruby: s.reverse
来源：http://xfh.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://vrn.bbcook.cn

[E12] 统计某字符出现次数
来源：http://ree.gogol.net.cn

Py:   s.count("a")
来源：http://iow.pycfn.com

PHP:  substr_count($s, "a");
来源：http://rji.uphjek.com

JS:   s.split("a").length - 1
来源：http://vgg.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://vdu.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kom.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://pjh.nanxinkj.top

Ruby: s.count("a")
来源：http://ifx.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://ere.tarul.cn

[E13] 逐字符遍历
来源：http://jhi.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://lak.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sjn.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxm.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bjr.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zhq.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmr.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fyk.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qga.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://zuv.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nrs.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rei.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ber.xylfe.cn


<!-- 参考信息 -->