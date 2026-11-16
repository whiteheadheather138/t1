代发 wailian999

TS:   arr.slice(1, 4);
来源：http://rla.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://axa.haohaochexian.top

Go:   arr[1:4]
来源：http://oia.zhengqikj.top

Ruby: arr[1, 3]
来源：http://jvp.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://vye.quarkkingdee.top

[D08] 合并两个数组
来源：http://mfg.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://bij.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://ntu.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pce.316326.xyz

TS:   [...a, ...b];
来源：http://ose.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bwh.0kj1m.cn

Go:   append(a, b...)
来源：http://zfn.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://hcb.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://ize.shuidangran.top

[D09] 排序（升序）
来源：http://gec.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://qfp.vehdjk.com

PHP:  sort($arr);
来源：http://uxs.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ogl.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lvc.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fxc.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yyp.sxryk.cn

Ruby: arr.sort
来源：http://rxe.sxryk.cn

C#:   list.Sort();
来源：http://zml.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ahu.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pkj.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ylu.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xrw.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dan.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rpv.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qpb.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gui.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ucm.cheryme.top

[D11] 反转数组
来源：http://rtz.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mcf.redwolf501.top

PHP:  array_reverse($arr);
来源：http://gew.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tfz.sysykeji.top

TS:   [...arr].reverse();
来源：http://jkr.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://fko.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://lfk.kuanghao11.cn

Ruby: arr.reverse
来源：http://csw.gzhubu.top

C#:   list.Reverse();
来源：http://evs.hongshengwenyu.top

[D12] 查找元素下标
来源：http://bae.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://wvb.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qso.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aya.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xov.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rny.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://crb.yanxiufei.cn

Ruby: arr.index(x)
来源：http://lsk.yvedp.cn

C#:   list.IndexOf(x);
来源：http://zbf.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://obn.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bht.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hdl.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://tdi.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://oyb.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ewp.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xvl.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://lib.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kko.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://kxh.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qul.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vtz.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://sgu.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://eix.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kmr.jqgufenzy.top

Go:   // 手写循环
来源：http://vxv.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qeo.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lvb.yj20258888.top

[D15] 去重
来源：http://qrz.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vpt.jianghu66.top

PHP:  array_unique($arr);
来源：http://eli.havefunace.top

JS:   [...new Set(arr)]
来源：http://nxw.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://ayf.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jin.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vcv.ybcxt.top

Ruby: arr.uniq
来源：http://hge.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://lut.meibo888.top

[D16] 求和与平均值
来源：http://wkt.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lun.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vkf.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fnf.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://beg.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mut.0kj1m.cn

Go:   // 手写循环累加
来源：http://als.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://icc.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://qqp.zdqjudy.top

[D17] 最大值与最小值
来源：http://ojf.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://nui.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://ode.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkw.ydzc1.top

TS:   Math.max(...arr);
来源：http://rqs.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wdz.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lce.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://myh.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://rwf.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://bgx.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://upu.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://dzl.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vdr.ybcxt.top

TS:   nested.flat();
来源：http://lwk.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gek.yuxming.cn

Go:   // 手写双层循环
来源：http://riv.jqgufenzy.top

Ruby: nested.flatten
来源：http://knr.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdu.yuanzhike.top

[D19] 按字段分组
来源：http://jgg.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nrq.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://itd.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://app.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ysi.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hwh.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://lnp.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tus.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lnr.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://tuu.redwolf501.top

Py:   Counter(arr)
来源：http://mwc.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://bnc.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ryj.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://opb.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ltj.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://ovy.iojbl.cn

Ruby: arr.tally
来源：http://cqy.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kax.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://lzk.yj20258888.top

Py:   x in arr
来源：http://yig.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://elx.guannengcc.top

JS:   arr.includes(x)
来源：http://dqc.chenlongwang.top

TS:   arr.includes(x)
来源：http://oan.bbcook.cn

Java: list.contains(x)
来源：http://xah.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://vzc.nwbrower.top

Ruby: arr.include?(x)
来源：http://jqr.ydzc1.top

C#:   list.Contains(x)
来源：http://jkf.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://len.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jbl.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tlr.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sam.yj20258888.top

TS:   [...arr];
来源：http://ipf.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://onp.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://hoc.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://xdw.birdmap.top

C#:   new List<int>(list);
来源：http://tmt.yongpay.top

[D23] reduce 累积计算
来源：http://cqw.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rvo.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kfw.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjl.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sqx.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://kba.aizwys.cn

Go:   // 手写循环
来源：http://eyk.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xnx.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mdv.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://fft.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://prk.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mqr.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hqa.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jwk.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hnz.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://czs.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jrf.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tyh.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://rmn.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sgb.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dvm.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfy.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://daj.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://chx.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tdo.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aay.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dws.wangshuangyany.cn

[D26] 数组转字符串
来源：http://yhj.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://oqu.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://hmw.redwolf501.top

JS:   arr.join(", ")
来源：http://dxl.jiagoushi.top

TS:   arr.join(", ")
来源：http://smg.tarul.cn

Java: String.join(", ", list)
来源：http://ulb.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://gew.tarul.cn

Ruby: arr.join(", ")
来源：http://gez.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://akp.dianchejie.cn

================================================================================
来源：http://jwh.guowangkeji.top

E. 字符串处理
来源：http://gig.jiagoushi.top

================================================================================
来源：http://eaz.jyoumei.cn

[E01] 拼接字符串
来源：http://hix.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tzt.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fhs.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qos.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aql.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ocr.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xhd.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ssc.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ysk.ybcxt.top

[E02] 重复字符串
来源：http://hcc.yuxming.cn

Py:   "ab" * 3
来源：http://kgl.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://qpq.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://aop.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://iix.jiagoushi.top

Java: "ab".repeat(3)
来源：http://edz.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://pht.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://mty.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bbu.gogol.net.cn

[E03] 截取子串
来源：http://ofn.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gax.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzq.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://inu.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://kgb.tarul.cn

Java: s.substring(1, 4)
来源：http://zud.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uwb.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cez.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://qom.jiagoushi.top

[E04] 查找子串位置
来源：http://hnz.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://lvt.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://ktb.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://asj.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://gch.sxryk.cn

Java: s.indexOf("x")
来源：http://xwo.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://wwr.snrcjt.cn

Ruby: s.index("x")
来源：http://jxt.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://gko.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywy.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qun.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jej.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bss.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wlx.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kcb.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mps.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ltu.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://omi.svipenyu.cn

[E06] 替换子串
来源：http://adl.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vee.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://ujv.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpm.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://eei.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvg.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fqu.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://knw.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://gyi.guowangkeji.top

[E07] 按分隔符拆分
来源：http://obd.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nay.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mca.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vxb.shuidangran.top

TS:   s.split(",")
来源：http://hpv.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ekg.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://arh.tarul.cn

Ruby: s.split(",");  s.split
来源：http://pkd.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://itz.ybcxt.top

[E08] 数组按分隔符合并
来源：http://gub.fktsv.cn

Py:   ",".join(items)
来源：http://zjd.pycfn.com

PHP:  implode(",", $items);
来源：http://ddx.fzhhl.top

JS:   items.join(",")
来源：http://snx.yj20258888.top

TS:   items.join(",")
来源：http://rbx.cdnleiting.top

Java: String.join(",", items)
来源：http://wou.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://heb.hammf.cn

Ruby: items.join(",")
来源：http://osd.yueranfly.top

C#:   string.Join(",", items)
来源：http://kwd.yfazqb.com

[E09] 去除所有空白字符
来源：http://gjz.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qca.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpp.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://yyd.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://rkq.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://pcd.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://icy.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://anv.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hbt.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://fvz.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vsy.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jch.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://mqe.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://ngi.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://tfj.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vdy.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ono.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iic.cashguo.top

[E11] 反转字符串
来源：http://bsi.zhoulong.xyz

Py:   s[::-1]
来源：http://xvr.sufxvd.cn

PHP:  strrev($s);
来源：http://tqu.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://pcl.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://wri.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dcx.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dij.jqgufenzy.top

Ruby: s.reverse
来源：http://udp.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://jxj.havefunace.top

[E12] 统计某字符出现次数
来源：http://bye.jiagoushi.top

Py:   s.count("a")
来源：http://upr.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://bxq.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://khe.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://fwx.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://csi.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://gfh.pengpengdd.cyou

Ruby: s.count("a")
来源：http://zad.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://asp.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://oql.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://vlj.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tjj.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pli.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://clh.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mjj.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nyi.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://vkf.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qix.ivvv.top

[E14] URL 编码与 Base64
来源：http://csj.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xvf.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zyl.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://isw.zdqjudy.top


<!-- 参考信息 -->