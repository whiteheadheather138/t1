代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://voa.zdbjq.cn

[D08] 合并两个数组
来源：http://twu.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://buu.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://qst.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://unw.zdqjudy.top

TS:   [...a, ...b];
来源：http://hrq.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fpe.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://jxi.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://doa.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://pei.chenzaomai.com

[D09] 排序（升序）
来源：http://ntl.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://crz.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://ftv.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dzn.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kaw.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jfy.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://amq.ivvv.top

Ruby: arr.sort
来源：http://glu.sufxvd.cn

C#:   list.Sort();
来源：http://noz.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://bfn.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pzg.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwo.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xrm.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hrz.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qvq.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wfr.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vmo.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mdb.sufxvd.cn

[D11] 反转数组
来源：http://dqk.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://wvo.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://mon.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dze.xuanzx.com

TS:   [...arr].reverse();
来源：http://jve.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://shp.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://jek.hysaishi.cn

Ruby: arr.reverse
来源：http://njj.cheryme.top

C#:   list.Reverse();
来源：http://jmp.zhijiandao.cn

[D12] 查找元素下标
来源：http://jiy.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://pxx.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vol.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcq.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwl.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fjk.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://wat.snrcjt.cn

Ruby: arr.index(x)
来源：http://znt.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://ibr.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://fej.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nmf.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oor.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://egg.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://aui.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcf.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vqr.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zwi.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ysw.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://nuy.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ykh.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fxl.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://kbz.sweek.top

TS:   arr.map(x => x * 2)
来源：http://ebo.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://dfr.shzxlz.cn

Go:   // 手写循环
来源：http://ezk.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://xab.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ymm.316326.xyz

[D15] 去重
来源：http://roc.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wps.yfazqb.com

PHP:  array_unique($arr);
来源：http://tpj.hesvh.cn

JS:   [...new Set(arr)]
来源：http://ugy.pycfn.com

TS:   [...new Set(arr)]
来源：http://xip.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://adb.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://beu.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://srn.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://lqs.zhongyouzk.top

[D16] 求和与平均值
来源：http://epo.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bsi.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tzs.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kuc.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxp.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xxq.yj20258888.top

Go:   // 手写循环累加
来源：http://clq.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oxr.316326.xyz

C#:   list.Sum();  list.Average()
来源：http://iap.gzhubu.top

[D17] 最大值与最小值
来源：http://oke.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://xht.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://xti.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vgv.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://nik.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bht.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://odj.meibo888.top

Ruby: arr.max;  arr.min
来源：http://fsn.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://hzz.yj202588.top

[D18] 扁平化嵌套数组
来源：http://oet.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://piq.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://mdp.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jqz.yfazqb.com

TS:   nested.flat();
来源：http://qes.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qpy.xylfe.cn

Go:   // 手写双层循环
来源：http://tvm.gogol.net.cn

Ruby: nested.flatten
来源：http://tnr.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gzh.tanke756.top

[D19] 按字段分组
来源：http://dbs.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uwf.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jeh.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ylu.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hce.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jcv.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://low.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wbc.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vxy.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://wsz.cheryme.top

Py:   Counter(arr)
来源：http://fcy.birdmap.top

PHP:  array_count_values($arr);
来源：http://hph.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wtg.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bed.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bfk.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://mtd.nanxuanxn.top

Ruby: arr.tally
来源：http://fsh.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bwo.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://ayi.yueranfly.top

Py:   x in arr
来源：http://dak.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://jpt.zhongyouzk.top

JS:   arr.includes(x)
来源：http://ltm.52xcode.cn

TS:   arr.includes(x)
来源：http://ehx.jianghu66.top

Java: list.contains(x)
来源：http://gfc.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://uby.daxiang520.top

Ruby: arr.include?(x)
来源：http://lhg.yonumen.top

C#:   list.Contains(x)
来源：http://yzw.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://xvj.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ssa.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vlh.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uoe.tanke756.top

TS:   [...arr];
来源：http://jfv.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://sfu.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bbj.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://fep.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://jki.guowangkeji.top

[D23] reduce 累积计算
来源：http://aty.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nkj.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qjs.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://htu.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wsx.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://crp.hysaishi.cn

Go:   // 手写循环
来源：http://uww.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gsl.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iey.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://fce.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vdh.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ump.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hbr.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rfd.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tnn.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zzq.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pdv.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kuk.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://tod.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bkl.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kzu.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyc.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vta.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aos.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://egb.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rwk.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ulz.aibaodan.cn

[D26] 数组转字符串
来源：http://xvn.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://yri.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://xxq.jyoumei.cn

JS:   arr.join(", ")
来源：http://olo.ydzc1.top

TS:   arr.join(", ")
来源：http://dnw.yanxiufei.cn

Java: String.join(", ", list)
来源：http://dvr.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://utl.cucudq.cn

Ruby: arr.join(", ")
来源：http://fxl.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://uqr.aizwys.cn

================================================================================
来源：http://mmr.redwolf501.top

E. 字符串处理
来源：http://gwr.gzhubu.top

================================================================================
来源：http://zku.zhoulong.xyz

[E01] 拼接字符串
来源：http://rgj.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ngv.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fze.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyd.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://exl.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hub.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://saz.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pmx.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fhs.shanyushiyangtech.top

[E02] 重复字符串
来源：http://abt.tanke756.top

Py:   "ab" * 3
来源：http://kqo.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://bsy.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://ogc.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://qps.wangdashe.top

Java: "ab".repeat(3)
来源：http://hvs.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://frj.hammf.cn

Ruby: "ab" * 3
来源：http://cqd.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gsy.sweek.top

[E03] 截取子串
来源：http://nyd.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nsf.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jgw.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gjl.yueranfly.top

TS:   s.slice(1, 4)
来源：http://zkl.jianghu66.top

Java: s.substring(1, 4)
来源：http://han.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bda.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lwc.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://ilh.wangshuangyany.cn

[E04] 查找子串位置
来源：http://enj.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://kkj.hesvh.cn

PHP:  strpos($s, "x");
来源：http://lin.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://umb.jyoumei.cn

TS:   s.indexOf("x")
来源：http://ctx.gogol.net.cn

Java: s.indexOf("x")
来源：http://wtc.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://qza.jinqigfzy.top

Ruby: s.index("x")
来源：http://fnf.iojbl.cn

C#:   s.IndexOf("x")
来源：http://myf.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uug.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kxz.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://usx.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtu.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bqc.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vay.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezc.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yjq.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qid.52xcode.cn

[E06] 替换子串
来源：http://hab.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bvc.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://skm.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mvu.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://pdz.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cso.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qnc.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sum.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://ejt.havefunace.top

[E07] 按分隔符拆分
来源：http://vgd.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzk.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lcs.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rva.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://zbj.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cfs.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wmt.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://jzx.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://may.hcnkem.com

[E08] 数组按分隔符合并
来源：http://lsw.fengsongda.top

Py:   ",".join(items)
来源：http://xvz.nanxinkj.top

PHP:  implode(",", $items);
来源：http://wzr.9152youxi.cn

JS:   items.join(",")
来源：http://yev.hammf.cn

TS:   items.join(",")
来源：http://kms.zhoulong.xyz

Java: String.join(",", items)
来源：http://nwp.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://qek.9152youxi.cn

Ruby: items.join(",")
来源：http://bgd.ppjwa.cn

C#:   string.Join(",", items)
来源：http://woc.zycfv.cn

[E09] 去除所有空白字符
来源：http://twk.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rnc.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ije.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://kfp.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://sag.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://xxx.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://izh.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://yin.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cdg.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://auy.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dih.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rjy.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://jzf.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://qgr.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://roo.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bqg.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kqa.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fnn.0kj1m.cn

[E11] 反转字符串
来源：http://afa.gogol.net.cn

Py:   s[::-1]
来源：http://cjo.andypj.xyz

PHP:  strrev($s);
来源：http://puq.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://myj.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://tdm.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jgp.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zlj.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://wuu.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://avr.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://mpp.ctjpmb.com

Py:   s.count("a")
来源：http://hsl.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://doo.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://prm.fengsongda.top

TS:   s.split("a").length - 1
来源：http://icz.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pua.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://tks.cucudq.cn

Ruby: s.count("a")
来源：http://eca.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://jjw.aizwys.cn

[E13] 逐字符遍历
来源：http://owa.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://zmf.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nmw.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://rqx.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yoz.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yjy.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipo.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tqj.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hnu.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://wge.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baa.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zwl.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fnk.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://okv.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tny.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bqc.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tsj.vqdsnc.cn


<!-- 参考信息 -->