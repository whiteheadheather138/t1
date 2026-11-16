代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://whu.zhijiandao.cn

[D08] 合并两个数组
来源：http://elj.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://pjh.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://ncw.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ena.jinqigufen.top

TS:   [...a, ...b];
来源：http://fri.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vvr.bbcook.cn

Go:   append(a, b...)
来源：http://ati.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://rop.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://fte.chenjidiqi.icu

[D09] 排序（升序）
来源：http://mde.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://sav.zhijiandao.cn

PHP:  sort($arr);
来源：http://qtm.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wnp.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://azu.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jcn.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://izl.yanxiufei.cn

Ruby: arr.sort
来源：http://ifv.shuidangran.top

C#:   list.Sort();
来源：http://vfs.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zwb.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sqx.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://skd.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oxy.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivh.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lqv.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufp.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://apr.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hfa.hongshengwenyu.top

[D11] 反转数组
来源：http://bue.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yoe.ydzc1.top

PHP:  array_reverse($arr);
来源：http://xeo.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mzz.ehwqpu.com

TS:   [...arr].reverse();
来源：http://kau.wangdashe.top

Java: Collections.reverse(list);
来源：http://ict.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://cyw.nanxuanxn.top

Ruby: arr.reverse
来源：http://yub.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://ugp.zhengqikj.top

[D12] 查找元素下标
来源：http://yiv.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://kvi.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://itx.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ssx.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://txr.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://msq.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://qxm.yj20258888.top

Ruby: arr.index(x)
来源：http://wlg.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://seq.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://ely.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://luu.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryw.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://lyh.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://hze.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://epr.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vts.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://cfp.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lth.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://vfl.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tti.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lgw.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://zzk.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://ahh.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://yya.guannengcc.top

Go:   // 手写循环
来源：http://nem.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tya.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dsg.cdnleiting.top

[D15] 去重
来源：http://bmo.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eon.fktsv.cn

PHP:  array_unique($arr);
来源：http://fat.zycfv.cn

JS:   [...new Set(arr)]
来源：http://cwq.uphjek.com

TS:   [...new Set(arr)]
来源：http://iyb.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tal.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bza.xinyue.icu

Ruby: arr.uniq
来源：http://yzj.uphjek.com

C#:   list.Distinct().ToList()
来源：http://edd.uphjek.com

[D16] 求和与平均值
来源：http://djw.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydx.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qyd.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mju.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tud.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ima.hnxiangtu.top

Go:   // 手写循环累加
来源：http://pma.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rxr.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://wwx.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://cxl.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://rff.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://vkh.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dkc.yj20258.top

TS:   Math.max(...arr);
来源：http://exg.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cmp.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zzw.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://oqu.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://gyu.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://rks.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fdw.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://zlv.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tkw.fanxiaobao.xyz

TS:   nested.flat();
来源：http://ayw.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mlx.zhongyouzk.top

Go:   // 手写双层循环
来源：http://xij.tian-w.cn

Ruby: nested.flatten
来源：http://ugf.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbk.yvedp.cn

[D19] 按字段分组
来源：http://nyz.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qeu.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oso.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bmi.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oda.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ehn.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://fpu.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tko.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://scl.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://qux.nwbrower.top

Py:   Counter(arr)
来源：http://orb.sweek.top

PHP:  array_count_values($arr);
来源：http://axk.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wol.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltf.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mhx.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://odz.yuxming.cn

Ruby: arr.tally
来源：http://eyy.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fxr.jianghu66.top

[D21] 判断是否包含某元素
来源：http://pcc.zycfv.cn

Py:   x in arr
来源：http://aun.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://onu.tian-w.cn

JS:   arr.includes(x)
来源：http://nio.vqdsnc.cn

TS:   arr.includes(x)
来源：http://ziy.52xcode.cn

Java: list.contains(x)
来源：http://ycd.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://ldm.xziqi.cn

Ruby: arr.include?(x)
来源：http://xvl.ctjpmb.com

C#:   list.Contains(x)
来源：http://mcy.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://tmn.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rhw.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yfx.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kms.jlsjyb.cn

TS:   [...arr];
来源：http://vpe.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://urb.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zhw.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://hap.gogol.net.cn

C#:   new List<int>(list);
来源：http://sqv.9152youxi.cn

[D23] reduce 累积计算
来源：http://viu.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://khu.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://byq.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxq.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dgc.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cwh.tanke756.top

Go:   // 手写循环
来源：http://tjl.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcf.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ebu.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://pas.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hyl.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abf.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jge.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ioa.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jvd.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xou.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vhe.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://afu.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://tht.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cma.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oud.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tuo.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kgz.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://unn.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vox.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://flo.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ohs.shuidangran.top

[D26] 数组转字符串
来源：http://pzs.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://lhd.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://pfq.xziqi.cn

JS:   arr.join(", ")
来源：http://pof.smart0.xyz

TS:   arr.join(", ")
来源：http://sai.hysaishi.cn

Java: String.join(", ", list)
来源：http://mpg.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://img.dianchejie.cn

Ruby: arr.join(", ")
来源：http://wor.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://aaz.jqgufenzy.top

================================================================================
来源：http://ttz.jyoumei.cn

E. 字符串处理
来源：http://pld.zdbjq.cn

================================================================================
来源：http://wzd.meibo888.top

[E01] 拼接字符串
来源：http://mqj.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yqs.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ovh.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qjk.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddf.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jhv.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sph.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hsb.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kph.cucudq.cn

[E02] 重复字符串
来源：http://gts.dashuyun.cn

Py:   "ab" * 3
来源：http://fbz.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://bdf.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://nvb.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://uwb.fehbvm.com

Java: "ab".repeat(3)
来源：http://qkz.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://cje.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://mns.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lmn.ehwqpu.com

[E03] 截取子串
来源：http://tnw.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ebf.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jjb.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zyd.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://hid.tian-w.cn

Java: s.substring(1, 4)
来源：http://onx.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pgn.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://flo.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://kfy.ybcxt.top

[E04] 查找子串位置
来源：http://itl.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://ysf.hcnkem.com

PHP:  strpos($s, "x");
来源：http://rhd.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://snz.haohaochexian.top

TS:   s.indexOf("x")
来源：http://vbq.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://vyy.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://tsr.c1oappe.top

Ruby: s.index("x")
来源：http://esc.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://qdg.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jjh.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dty.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kgo.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tby.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xja.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gam.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mas.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dew.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ekj.xinyue.icu

[E06] 替换子串
来源：http://nwx.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://byt.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://jtt.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aeb.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://yix.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vlp.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wen.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://njz.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://fws.yvedp.cn

[E07] 按分隔符拆分
来源：http://yqg.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://onf.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kzw.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://yoi.hnxiangtu.top

TS:   s.split(",")
来源：http://jfn.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://mvn.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qln.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://gyp.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ves.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://xyf.tanke756.top

Py:   ",".join(items)
来源：http://faf.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://vac.kuanghao11.cn

JS:   items.join(",")
来源：http://dbf.tanke756.top

TS:   items.join(",")
来源：http://dvw.yj20258.top

Java: String.join(",", items)
来源：http://ipc.yj20258.top

Go:   strings.Join(items, ",")
来源：http://nhc.hywenlv.cn

Ruby: items.join(",")
来源：http://cec.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://lei.sxryk.cn

[E09] 去除所有空白字符
来源：http://ses.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gek.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xhz.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://pmf.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://ljw.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://frg.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gkw.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://lnj.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pce.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://ahn.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ben.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dsq.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://yjy.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://bwn.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://xdz.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://qys.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hfx.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gnw.yanxiufei.cn

[E11] 反转字符串
来源：http://wqp.havefunace.top

Py:   s[::-1]
来源：http://wqq.xziqi.cn

PHP:  strrev($s);
来源：http://udh.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://ipg.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://rip.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bjr.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ggi.sxryk.cn

Ruby: s.reverse
来源：http://ezq.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mmn.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://gky.chenzaomai.com

Py:   s.count("a")
来源：http://xxj.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://rkc.daria6918.cn

JS:   s.split("a").length - 1
来源：http://tpd.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://can.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qij.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://pqz.guannengcc.top

Ruby: s.count("a")
来源：http://ezo.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://swz.gotoacloud.top

[E13] 逐字符遍历
来源：http://gaa.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://cio.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://taa.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mzh.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hxn.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tyx.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uev.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kem.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gwj.gzhubu.top

[E14] URL 编码与 Base64
来源：http://xvw.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ijx.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ryj.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pct.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zbj.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lym.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://onk.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://prd.9152youxi.cn


<!-- 参考信息 -->