代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eaa.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://njj.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://qnl.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://inb.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://zqf.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vry.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pat.ydzc1.top

[D06] 数组长度
来源：http://btn.fktsv.cn

Py:   len(arr)
来源：http://cqu.gogol.net.cn

PHP:  count($arr);
来源：http://odf.zhoulong.xyz

JS:   arr.length
来源：http://huk.jyoumei.cn

TS:   arr.length
来源：http://iho.jlsjyb.cn

Java: list.size();
来源：http://yjs.yongpay.top

Go:   len(arr)
来源：http://tur.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://rdp.snrcjt.cn

C#:   list.Count;
来源：http://qey.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://zuw.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyb.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://lkm.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://sad.birdmap.top

TS:   arr.slice(1, 4);
来源：http://cla.iojbl.cn

Java: list.subList(1, 4);
来源：http://gci.yuanzhike.top

Go:   arr[1:4]
来源：http://btq.bjfxy.top

Ruby: arr[1, 3]
来源：http://kyx.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://fyp.yuanzhike.top

[D08] 合并两个数组
来源：http://wdg.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://awx.yj202588.top

PHP:  array_merge($a, $b);
来源：http://ljv.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rih.0kj1m.cn

TS:   [...a, ...b];
来源：http://ely.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jbq.smart0.xyz

Go:   append(a, b...)
来源：http://sqt.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://tgm.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://xdi.mhx1999.top

[D09] 排序（升序）
来源：http://noh.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://tbs.yonumen.top

PHP:  sort($arr);
来源：http://ane.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://buc.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bhh.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oor.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://agl.sxryk.cn

Ruby: arr.sort
来源：http://tuf.cheryme.top

C#:   list.Sort();
来源：http://exp.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xoa.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nao.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lrx.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsg.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iuh.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xhw.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wqh.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blz.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wax.nanxuanxn.top

[D11] 反转数组
来源：http://tqf.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://bsy.smart0.xyz

PHP:  array_reverse($arr);
来源：http://adv.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://weu.cheryme.top

TS:   [...arr].reverse();
来源：http://nzc.gogol.net.cn

Java: Collections.reverse(list);
来源：http://pig.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://jcp.bjfxy.top

Ruby: arr.reverse
来源：http://gsm.guowangkeji.top

C#:   list.Reverse();
来源：http://rme.dashuyun.cn

[D12] 查找元素下标
来源：http://ucu.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://quu.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ozh.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gbf.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wqb.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sjw.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://rke.gaohongyu789.top

Ruby: arr.index(x)
来源：http://zqt.guannengcc.top

C#:   list.IndexOf(x);
来源：http://wxc.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://bap.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dlp.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ehm.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://mdy.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://wua.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bji.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wrp.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://dbm.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wtj.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://btn.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wrs.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cvq.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://rss.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://zmz.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://eck.meibo888.top

Go:   // 手写循环
来源：http://lqc.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gua.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://dku.svipenyu.cn

[D15] 去重
来源：http://awo.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kgv.mhx1999.top

PHP:  array_unique($arr);
来源：http://amp.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://ytw.fzhhl.top

TS:   [...new Set(arr)]
来源：http://hob.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ado.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://wcj.zdbjq.cn

Ruby: arr.uniq
来源：http://ixj.havefunace.top

C#:   list.Distinct().ToList()
来源：http://ppb.gogol.net.cn

[D16] 求和与平均值
来源：http://zkl.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kyn.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://krf.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ght.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lps.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sow.zhengqikj.top

Go:   // 手写循环累加
来源：http://wob.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://snm.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://zrl.sxryk.cn

[D17] 最大值与最小值
来源：http://uwi.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://ulu.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://bsq.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tzx.fehbvm.com

TS:   Math.max(...arr);
来源：http://evy.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lkc.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fvt.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://nzz.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://ppl.tarul.cn

[D18] 扁平化嵌套数组
来源：http://efl.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aos.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://ihq.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lpx.316326.xyz

TS:   nested.flat();
来源：http://qlm.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wel.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://mjq.xziqi.cn

Ruby: nested.flatten
来源：http://edq.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kni.iojbl.cn

[D19] 按字段分组
来源：http://gph.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vuz.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ecy.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://but.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hlu.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nyv.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://uge.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqr.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ehy.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://dux.fktsv.cn

Py:   Counter(arr)
来源：http://ljc.meibo888.top

PHP:  array_count_values($arr);
来源：http://lhr.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ota.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xkn.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gsz.wangdashe.top

Go:   // 手写 map[T]int
来源：http://fjd.pengpengdd.cyou

Ruby: arr.tally
来源：http://kxj.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tsw.yj20258888.top

[D21] 判断是否包含某元素
来源：http://amj.cashguo.top

Py:   x in arr
来源：http://zzc.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://gns.cucudq.cn

JS:   arr.includes(x)
来源：http://ohk.chenlongwang.top

TS:   arr.includes(x)
来源：http://ozq.yangfankeji.com

Java: list.contains(x)
来源：http://ktx.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://sgx.yueranfly.top

Ruby: arr.include?(x)
来源：http://dxp.gogol.net.cn

C#:   list.Contains(x)
来源：http://rgo.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://dlw.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vlp.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpv.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wci.smart0.xyz

TS:   [...arr];
来源：http://mpe.andypj.xyz

Java: new ArrayList<>(list);
来源：http://snb.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iez.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://wbg.xuanzx.com

C#:   new List<int>(list);
来源：http://tmr.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://lys.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://emw.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ahd.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwu.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znf.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://igj.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://oue.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://svn.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsr.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://wrn.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://buy.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erb.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ezp.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wjn.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ywd.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tzx.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cgf.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lfv.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://uxp.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yhn.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tfk.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ymt.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlb.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzb.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uqp.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ctd.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wnd.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://fvf.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://ury.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://ron.gotoacloud.top

JS:   arr.join(", ")
来源：http://jmv.ydzc1.top

TS:   arr.join(", ")
来源：http://tay.ctjpmb.com

Java: String.join(", ", list)
来源：http://zum.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://lzh.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://qbg.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://ofv.shanyushiyangkeji.top

================================================================================
来源：http://ydj.chenzaomai.com

E. 字符串处理
来源：http://qyd.fengsongda.top

================================================================================
来源：http://asr.jiagoushi.top

[E01] 拼接字符串
来源：http://fyj.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fqt.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yjj.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jxs.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpp.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://szj.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dew.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jwa.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mbz.andypj.xyz

[E02] 重复字符串
来源：http://wlk.tanke756.top

Py:   "ab" * 3
来源：http://lpm.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://oiw.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://nrq.xylfe.cn

TS:   "ab".repeat(3)
来源：http://uzg.guowangkeji.top

Java: "ab".repeat(3)
来源：http://aer.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://tnc.nanxinkj.top

Ruby: "ab" * 3
来源：http://ruz.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://svb.shangyingyoupin.top

[E03] 截取子串
来源：http://ahq.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://srs.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ktw.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://doe.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://esm.ydzc1.top

Java: s.substring(1, 4)
来源：http://ewr.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mxz.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ozk.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://eay.ppjwa.cn

[E04] 查找子串位置
来源：http://jrd.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://iqv.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://qec.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wlm.cashguo.top

TS:   s.indexOf("x")
来源：http://nsg.ydzc1.top

Java: s.indexOf("x")
来源：http://wpg.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://mya.redwolf501.top

Ruby: s.index("x")
来源：http://nwl.havefunace.top

C#:   s.IndexOf("x")
来源：http://ekg.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://der.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xvq.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uee.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sko.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://diz.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://niu.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gmw.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://adq.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qrr.yj202588.top

[E06] 替换子串
来源：http://mbw.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ili.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://gke.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ihm.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://jgy.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ust.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qvs.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iyx.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://kwl.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://dhw.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://thc.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yox.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iuo.shuidangran.top

TS:   s.split(",")
来源：http://ypg.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ddq.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vnu.havefunace.top

Ruby: s.split(",");  s.split
来源：http://eip.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hvq.52xcode.cn

[E08] 数组按分隔符合并
来源：http://pfu.yongpay.top

Py:   ",".join(items)
来源：http://xof.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://teo.xuetiantiany.cn

JS:   items.join(",")
来源：http://nqt.fengsongda.top

TS:   items.join(",")
来源：http://bmn.yj202588.top

Java: String.join(",", items)
来源：http://ros.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://tsu.hammf.cn

Ruby: items.join(",")
来源：http://tez.chenlongwang.top

C#:   string.Join(",", items)
来源：http://mek.zycfv.cn

[E09] 去除所有空白字符
来源：http://hdz.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqq.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kko.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://vnl.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://lim.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://uoo.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mxc.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kgz.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://noy.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://qpt.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qix.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tws.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://hom.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://ahf.yongpay.top

Java: String.format("%03d", 7)
来源：http://uiw.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ezk.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gjt.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xdm.hammf.cn

[E11] 反转字符串
来源：http://bkn.chenzaomai.com

Py:   s[::-1]
来源：http://ujz.sjlbkw.cn

PHP:  strrev($s);
来源：http://yae.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://tmp.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://doq.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ztn.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sno.zhixingplan.top

Ruby: s.reverse
来源：http://ppq.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://zuy.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://xaf.hongshengwenyu.top

Py:   s.count("a")
来源：http://rir.hammf.cn


<!-- 参考信息 -->