代发 wailian999

[D07] 切片 / 取子数组
来源：http://bhi.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ads.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://eed.yj202588.top

JS:   arr.slice(1, 4);
来源：http://lgh.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://ped.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://fgn.tian-w.cn

Go:   arr[1:4]
来源：http://wnj.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://fjz.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://nuh.yj20258888.top

[D08] 合并两个数组
来源：http://opx.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://hpg.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://kcl.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jrz.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://aqa.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cjg.ppjwa.cn

Go:   append(a, b...)
来源：http://hqk.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://yss.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://rvw.birdmap.top

[D09] 排序（升序）
来源：http://ddb.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://krm.wangdashe.top

PHP:  sort($arr);
来源：http://qzh.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oru.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://xyn.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hwt.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ytn.gaohongyu789.top

Ruby: arr.sort
来源：http://zpv.hfpthk.cn

C#:   list.Sort();
来源：http://ykw.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qya.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nap.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dxx.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tca.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjp.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqo.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uuq.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jni.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://imj.snrcjt.cn

[D11] 反转数组
来源：http://epy.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kfp.xziqi.cn

PHP:  array_reverse($arr);
来源：http://dog.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dnb.hywenlv.cn

TS:   [...arr].reverse();
来源：http://uei.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://wep.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://rnv.daria6918.cn

Ruby: arr.reverse
来源：http://auk.sysykeji.top

C#:   list.Reverse();
来源：http://uip.wangshuangyany.cn

[D12] 查找元素下标
来源：http://dle.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://kla.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://thy.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fah.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kje.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lzm.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://imm.yj202588.top

Ruby: arr.index(x)
来源：http://kez.xinyue.icu

C#:   list.IndexOf(x);
来源：http://now.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://ifb.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wgb.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xnl.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://rso.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://kyk.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vpt.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nsl.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://klw.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://veu.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://qem.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cqk.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tun.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://mcc.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://uwm.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ioo.chenjidiqi.icu

Go:   // 手写循环
来源：http://ofq.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ypr.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cfs.zhiwuduotai.top

[D15] 去重
来源：http://fiv.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://myw.yj202588.top

PHP:  array_unique($arr);
来源：http://cvq.yfazqb.com

JS:   [...new Set(arr)]
来源：http://vta.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://vnw.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ahm.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oyc.smart0.xyz

Ruby: arr.uniq
来源：http://phq.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://npk.gaohongyu789.top

[D16] 求和与平均值
来源：http://tpu.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mmu.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fag.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hgh.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://urh.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pdm.zdqjudy.top

Go:   // 手写循环累加
来源：http://fpp.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qkp.sweek.top

C#:   list.Sum();  list.Average()
来源：http://tli.snrcjt.cn

[D17] 最大值与最小值
来源：http://avl.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://zyb.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://cot.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qea.smart0.xyz

TS:   Math.max(...arr);
来源：http://rvc.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wqo.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hwa.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://klh.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://tkx.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://qzn.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nkv.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://mud.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ahx.jinqigufen.top

TS:   nested.flat();
来源：http://kut.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lzt.yangfankeji.com

Go:   // 手写双层循环
来源：http://glz.cucudq.cn

Ruby: nested.flatten
来源：http://ggp.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://jpq.yvedp.cn

[D19] 按字段分组
来源：http://tjv.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ygp.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jpu.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qul.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://svo.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mdv.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://pjq.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fll.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dbn.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ydi.0kj1m.cn

Py:   Counter(arr)
来源：http://ske.tarul.cn

PHP:  array_count_values($arr);
来源：http://rtu.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vto.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uqo.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://out.ydzc1.top

Go:   // 手写 map[T]int
来源：http://ygj.zhiwuduotai.top

Ruby: arr.tally
来源：http://ull.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jos.fengsongda.top

[D21] 判断是否包含某元素
来源：http://xep.hcnkem.com

Py:   x in arr
来源：http://sbs.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://xki.nwbrower.top

JS:   arr.includes(x)
来源：http://vds.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://dxt.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://oif.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://pno.andypj.xyz

Ruby: arr.include?(x)
来源：http://lnh.yongpay.top

C#:   list.Contains(x)
来源：http://qkb.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://wle.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ksu.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ytd.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://koq.sxryk.cn

TS:   [...arr];
来源：http://jnf.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://jsj.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kti.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://lse.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://qvm.daria6918.cn

[D23] reduce 累积计算
来源：http://mon.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://afp.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swa.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tza.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://num.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdz.tarul.cn

Go:   // 手写循环
来源：http://vvm.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mtw.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dkd.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://vpe.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xca.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owr.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tqn.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fxx.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgh.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fnu.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qxv.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wxe.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://yko.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://isx.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://red.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://erb.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ksw.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jer.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gan.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zdh.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tdw.hcnkem.com

[D26] 数组转字符串
来源：http://hdi.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://tpc.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://ptq.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://cgd.yuxming.cn

TS:   arr.join(", ")
来源：http://ora.redwolf501.top

Java: String.join(", ", list)
来源：http://umg.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://ubo.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://tir.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://vpz.pengpengdd.cyou

================================================================================
来源：http://jso.vehdjk.com

E. 字符串处理
来源：http://eeb.shanyushiyangtech.top

================================================================================
来源：http://duh.gogol.net.cn

[E01] 拼接字符串
来源：http://nxx.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nzq.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ruc.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnn.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uoz.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://udt.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oek.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rav.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hge.jinghuilouyu.cn

[E02] 重复字符串
来源：http://hjy.iojbl.cn

Py:   "ab" * 3
来源：http://trz.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://djm.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://uon.cucudq.cn

TS:   "ab".repeat(3)
来源：http://rqg.hywenlv.cn

Java: "ab".repeat(3)
来源：http://son.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://tqt.svipenyu.cn

Ruby: "ab" * 3
来源：http://wuw.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oyj.jqgfzy.top

[E03] 截取子串
来源：http://wfv.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqc.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jjn.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dfw.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://dpo.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://obw.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://seq.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://aon.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://mje.quarkkingdee.top

[E04] 查找子串位置
来源：http://fym.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://idz.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://gcq.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gub.jianghu66.top

TS:   s.indexOf("x")
来源：http://rrp.shuidangran.top

Java: s.indexOf("x")
来源：http://uor.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://vke.ydjk.org.cn

Ruby: s.index("x")
来源：http://sbt.aizwys.cn

C#:   s.IndexOf("x")
来源：http://iks.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xsj.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gws.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nes.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iwo.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xdk.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://juj.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lgf.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nrx.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqm.bbcook.cn

[E06] 替换子串
来源：http://lix.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nuz.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://bvf.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://krx.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://yiz.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjj.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bya.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wnr.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://ohw.ctjpmb.com

[E07] 按分隔符拆分
来源：http://fgc.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eff.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lqm.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://czu.tianlin.xyz

TS:   s.split(",")
来源：http://xxn.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://qud.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://orp.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://ldj.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fgy.havefunace.top

[E08] 数组按分隔符合并
来源：http://ojf.ivvv.top

Py:   ",".join(items)
来源：http://ams.yj202588.top

PHP:  implode(",", $items);
来源：http://vwk.daria6918.cn

JS:   items.join(",")
来源：http://jhr.zhixingplan.top

TS:   items.join(",")
来源：http://upv.bjfxy.top

Java: String.join(",", items)
来源：http://xgr.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://rfn.tanke756.top

Ruby: items.join(",")
来源：http://mxv.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://nks.shuidangran.top

[E09] 去除所有空白字符
来源：http://jlp.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xfe.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rwu.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://qrs.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://zui.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://lth.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://piv.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://bqg.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jzv.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://jjs.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aqq.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xbo.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://fbs.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://gjb.cucudq.cn

Java: String.format("%03d", 7)
来源：http://dtn.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nzb.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbg.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jvc.chenjidiqi.icu

[E11] 反转字符串
来源：http://jqu.gogol.net.cn

Py:   s[::-1]
来源：http://puj.shangyingyoupin.top

PHP:  strrev($s);
来源：http://mwl.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://euv.tarul.cn

TS:   [...s].reverse().join("")
来源：http://bdr.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ntc.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wcp.uphjek.com

Ruby: s.reverse
来源：http://wbc.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zqy.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://rlg.svipenyu.cn

Py:   s.count("a")
来源：http://tqd.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://pnp.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://xss.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://ofe.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hjv.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://xiz.gaohongyu789.top

Ruby: s.count("a")
来源：http://vzt.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://xdu.yonumen.top

[E13] 逐字符遍历
来源：http://gah.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://dbz.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tsd.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vlh.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hdx.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vvu.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://asu.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lwy.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iwt.pycfn.com


<!-- 参考信息 -->