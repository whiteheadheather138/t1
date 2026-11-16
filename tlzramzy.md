代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjt.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wip.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://geh.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xjg.jqgfzy.top

[D11] 反转数组
来源：http://ypp.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://jet.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://omi.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cwj.yfazqb.com

TS:   [...arr].reverse();
来源：http://uag.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://vas.yj202588.top

Go:   slices.Reverse(arr)
来源：http://fym.pengpengdd.cyou

Ruby: arr.reverse
来源：http://zyy.shangyingyoupin.top

C#:   list.Reverse();
来源：http://iwj.dianchejie.cn

[D12] 查找元素下标
来源：http://xht.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://zkc.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uto.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayi.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gdv.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zqa.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://hfp.aizwys.cn

Ruby: arr.index(x)
来源：http://vlg.daria6918.cn

C#:   list.IndexOf(x);
来源：http://mlo.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://shd.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tbq.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hmf.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://zxt.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://enp.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pqg.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eav.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://foa.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://ngc.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://xzk.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://muv.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zou.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://lph.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://wxt.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzn.fzhhl.top

Go:   // 手写循环
来源：http://hxa.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lok.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zpl.xziqi.cn

[D15] 去重
来源：http://nqj.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lvv.tian-w.cn

PHP:  array_unique($arr);
来源：http://ybi.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://fmz.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://xoj.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jbt.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ciy.9152youxi.cn

Ruby: arr.uniq
来源：http://aqe.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://zzf.fehbvm.com

[D16] 求和与平均值
来源：http://nzl.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bdy.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ovx.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tqr.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://icr.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywo.zdbjq.cn

Go:   // 手写循环累加
来源：http://ybg.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ecs.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://nrg.cdnleiting.top

[D17] 最大值与最小值
来源：http://gbk.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://aev.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://lnp.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dub.0kj1m.cn

TS:   Math.max(...arr);
来源：http://vcl.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mrw.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ycr.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://vmp.havefunace.top

C#:   list.Max();  list.Min()
来源：http://yso.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://syg.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gjv.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://ojr.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dzl.daxiang520.top

TS:   nested.flat();
来源：http://tzq.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pal.hcnkem.com

Go:   // 手写双层循环
来源：http://efj.xziqi.cn

Ruby: nested.flatten
来源：http://spc.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qdl.feifeiyinyue.top

[D19] 按字段分组
来源：http://hux.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pmt.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vov.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vxq.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fky.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eno.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://air.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://saf.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hfu.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://rjq.yonumen.top

Py:   Counter(arr)
来源：http://bjv.yuxming.cn

PHP:  array_count_values($arr);
来源：http://xzm.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://loq.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gst.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ndu.hcnkem.com

Go:   // 手写 map[T]int
来源：http://eou.redwolf501.top

Ruby: arr.tally
来源：http://dyr.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dxz.tian-w.cn

[D21] 判断是否包含某元素
来源：http://akt.quarkkingdee.top

Py:   x in arr
来源：http://udy.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://kwi.jinqigufen.top

JS:   arr.includes(x)
来源：http://cis.bjfxy.top

TS:   arr.includes(x)
来源：http://rtz.jqgufenzy.top

Java: list.contains(x)
来源：http://itk.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://ywt.nwbrower.top

Ruby: arr.include?(x)
来源：http://hro.vehdjk.com

C#:   list.Contains(x)
来源：http://qwl.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://udc.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ruu.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dcp.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uom.jiagoushi.top

TS:   [...arr];
来源：http://kvv.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://oxq.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://abx.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://tpr.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://vrb.ctjpmb.com

[D23] reduce 累积计算
来源：http://sdm.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kps.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nuu.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqb.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lkm.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lwg.nanxinkj.top

Go:   // 手写循环
来源：http://hao.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gnp.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xqs.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://xvu.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eqb.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tcc.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bpc.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xae.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxw.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bjf.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ljj.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://byn.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://bge.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sze.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eaf.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://php.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pwc.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nxb.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rgn.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dlv.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vpj.andypj.xyz

[D26] 数组转字符串
来源：http://tka.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://uew.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://zsc.9152youxi.cn

JS:   arr.join(", ")
来源：http://nuz.c1oappe.top

TS:   arr.join(", ")
来源：http://kue.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://fwy.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://jzp.hammf.cn

Ruby: arr.join(", ")
来源：http://cbq.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://xzh.ywan-chungtsiang.top

================================================================================
来源：http://juy.mhx1999.top

E. 字符串处理
来源：http://svh.feifeiyinyue.top

================================================================================
来源：http://tlh.0kj1m.cn

[E01] 拼接字符串
来源：http://bne.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ozz.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mto.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://egk.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tey.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iji.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vap.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdc.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pzl.chenjidiqi.icu

[E02] 重复字符串
来源：http://tho.fzhhl.top

Py:   "ab" * 3
来源：http://mxz.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://tqe.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://jkm.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://uzr.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://zrj.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://efz.bbcook.cn

Ruby: "ab" * 3
来源：http://uzm.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nrn.ybcxt.top

[E03] 截取子串
来源：http://uda.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://agm.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cvn.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nyl.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://pui.jianghu66.top

Java: s.substring(1, 4)
来源：http://vdm.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fwb.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://ozq.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://jel.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://bfp.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://top.fzhhl.top

PHP:  strpos($s, "x");
来源：http://brb.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yye.fehbvm.com

TS:   s.indexOf("x")
来源：http://wle.0kj1m.cn

Java: s.indexOf("x")
来源：http://maf.yonumen.top

Go:   strings.Index(s, "x")
来源：http://kur.sweek.top

Ruby: s.index("x")
来源：http://rdb.meibo888.top

C#:   s.IndexOf("x")
来源：http://xrg.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mvx.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zem.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sxa.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zjf.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yke.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgd.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oqs.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fgf.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zxs.yvedp.cn

[E06] 替换子串
来源：http://xcm.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://atv.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://lhy.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ihg.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://ciy.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgp.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zsl.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://scd.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://fcz.dianchejie.cn

[E07] 按分隔符拆分
来源：http://qfl.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bfl.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://opt.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nbl.hcnkem.com

TS:   s.split(",")
来源：http://eqi.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://jdk.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://otc.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://awn.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fbt.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://nsq.bbcook.cn

Py:   ",".join(items)
来源：http://tvw.daxiang520.top

PHP:  implode(",", $items);
来源：http://euo.vqdsnc.cn

JS:   items.join(",")
来源：http://had.chenjidiqi.icu

TS:   items.join(",")
来源：http://pwd.aibaodan.cn

Java: String.join(",", items)
来源：http://syw.meibo888.top

Go:   strings.Join(items, ",")
来源：http://usa.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://kbs.hnqzz.top

C#:   string.Join(",", items)
来源：http://iap.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://rtw.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bxi.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xlb.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://omu.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://eja.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://gav.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jra.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://kao.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubq.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://yyh.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://krn.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qyu.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://gad.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://vuj.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://snt.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gsr.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://efv.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zni.feifeiyinyue.top

[E11] 反转字符串
来源：http://twl.snrcjt.cn

Py:   s[::-1]
来源：http://tyz.nanxuanxn.top

PHP:  strrev($s);
来源：http://xlo.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://ybc.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://smk.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://von.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xts.yvedp.cn

Ruby: s.reverse
来源：http://gko.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://wfy.yonumen.top

[E12] 统计某字符出现次数
来源：http://ivv.xziqi.cn

Py:   s.count("a")
来源：http://cht.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://cmk.guannengcc.top

JS:   s.split("a").length - 1
来源：http://vjm.epnwcf.com

TS:   s.split("a").length - 1
来源：http://cma.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qmf.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://trl.gogol.net.cn

Ruby: s.count("a")
来源：http://hay.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://amy.ybcxt.top

[E13] 逐字符遍历
来源：http://hds.316326.xyz

Py:   for ch in s: print(ch)
来源：http://hyo.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bnx.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://unx.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qmz.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vbj.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pzs.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://yck.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tjj.nwbrower.top

[E14] URL 编码与 Base64
来源：http://cpn.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://idp.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://shg.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oiw.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xca.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ixv.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://edu.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tcl.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sts.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://cpp.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tcc.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yqo.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mhd.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dte.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pam.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wza.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rxc.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wco.fehbvm.com

[E16] 数字千分位
来源：http://qoa.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://spi.epnwcf.com

PHP:  number_format(1234567);
来源：http://wcy.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wjj.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://blc.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nrc.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jxz.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qhk.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://hcs.birdmap.top

[E17] 首字母大写
来源：http://kcl.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qgw.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dcx.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vwv.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iac.fanxiaobao.xyz


<!-- 参考信息 -->