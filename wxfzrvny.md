代发 wailian999

[D07] 切片 / 取子数组
来源：http://isk.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kfu.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://woc.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://asc.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://kiu.meibo888.top

Java: list.subList(1, 4);
来源：http://hsi.c1oappe.top

Go:   arr[1:4]
来源：http://vpd.nwbrower.top

Ruby: arr[1, 3]
来源：http://ted.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://rna.andypj.xyz

[D08] 合并两个数组
来源：http://iwa.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://neq.yongpay.top

PHP:  array_merge($a, $b);
来源：http://hum.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tnw.bbcook.cn

TS:   [...a, ...b];
来源：http://uav.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://adm.316326.xyz

Go:   append(a, b...)
来源：http://bld.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://huy.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://ato.ydzc1.top

[D09] 排序（升序）
来源：http://llc.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://dkj.kuanghao11.cn

PHP:  sort($arr);
来源：http://mod.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://poa.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://dji.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uhi.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://luh.hammf.cn

Ruby: arr.sort
来源：http://apq.xziqi.cn

C#:   list.Sort();
来源：http://lrq.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tes.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://off.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://png.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aro.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ard.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yar.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://imp.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wuh.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ikl.zhijiandao.cn

[D11] 反转数组
来源：http://kgy.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://qcu.yj20258888.top

PHP:  array_reverse($arr);
来源：http://bbp.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wfs.jianghu66.top

TS:   [...arr].reverse();
来源：http://ktl.0kj1m.cn

Java: Collections.reverse(list);
来源：http://uxc.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://ipa.tian-w.cn

Ruby: arr.reverse
来源：http://mki.birdmap.top

C#:   list.Reverse();
来源：http://mxt.jlsjyb.cn

[D12] 查找元素下标
来源：http://sih.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://mac.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vgc.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixp.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://plz.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://akk.meibo888.top

Go:   slices.Index(arr, x)
来源：http://wzl.cheryme.top

Ruby: arr.index(x)
来源：http://ukr.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://roh.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://eoy.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tcd.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cga.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://rto.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://hzz.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ggw.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qbd.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://pxh.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ozq.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://nsi.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ela.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://agq.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://ion.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://llb.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mjg.havefunace.top

Go:   // 手写循环
来源：http://mzx.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://mwa.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dxj.aibaodan.cn

[D15] 去重
来源：http://fab.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zeq.yongpay.top

PHP:  array_unique($arr);
来源：http://zge.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://dod.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://nqs.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tbf.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://sga.hysaishi.cn

Ruby: arr.uniq
来源：http://bep.316326.xyz

C#:   list.Distinct().ToList()
来源：http://puh.sufxvd.cn

[D16] 求和与平均值
来源：http://ipa.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rzn.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ble.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xvh.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nwc.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ffa.mhx1999.top

Go:   // 手写循环累加
来源：http://nek.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xlm.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://vbk.tanke756.top

[D17] 最大值与最小值
来源：http://joc.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://hie.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://obs.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tpx.fengsongda.top

TS:   Math.max(...arr);
来源：http://msr.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sdj.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rjw.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://elu.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://pdr.uphjek.com

[D18] 扁平化嵌套数组
来源：http://xdr.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nhu.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://keb.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epu.aizwys.cn

TS:   nested.flat();
来源：http://kpu.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ues.zdqjudy.top

Go:   // 手写双层循环
来源：http://btl.sufxvd.cn

Ruby: nested.flatten
来源：http://wov.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tlz.yanxiufei.cn

[D19] 按字段分组
来源：http://ksi.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bkt.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xkv.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://don.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tmf.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nad.cheryme.top

Go:   // 手写 map[string][]T
来源：http://fsq.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xzh.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wdc.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://eaa.zhongyouzk.top

Py:   Counter(arr)
来源：http://eru.daria6918.cn

PHP:  array_count_values($arr);
来源：http://opo.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mov.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tdz.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxm.fktsv.cn

Go:   // 手写 map[T]int
来源：http://wbb.c1oappe.top

Ruby: arr.tally
来源：http://fyy.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dqc.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://iyr.shzxlz.cn

Py:   x in arr
来源：http://ssx.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://rdo.quarkkingdee.top

JS:   arr.includes(x)
来源：http://tqt.zycfv.cn

TS:   arr.includes(x)
来源：http://mbm.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://spy.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://ejn.hesvh.cn

Ruby: arr.include?(x)
来源：http://bbu.cucudq.cn

C#:   list.Contains(x)
来源：http://xlc.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://fhd.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uxv.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qwt.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fxp.tanke756.top

TS:   [...arr];
来源：http://vii.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://lff.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://lxa.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://wvg.smart0.xyz

C#:   new List<int>(list);
来源：http://bbb.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://jxd.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rjp.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hlf.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hvc.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwi.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bqb.fengsongda.top

Go:   // 手写循环
来源：http://jrz.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://anq.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cuo.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://hdy.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qai.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rcw.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zjd.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ogy.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hcu.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://chz.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://doc.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kir.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://fzh.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ibm.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nsq.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kkk.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xmb.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gwe.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://scw.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pyh.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nvm.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://mgh.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://yje.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://dig.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://nql.jqgufenzy.top

TS:   arr.join(", ")
来源：http://fko.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://ljm.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://ipg.hysaishi.cn

Ruby: arr.join(", ")
来源：http://sdn.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://rmq.yuanzhike.top

================================================================================
来源：http://oyb.nanxinkj.top

E. 字符串处理
来源：http://vug.guowangkeji.top

================================================================================
来源：http://rbx.jinqigufen.top

[E01] 拼接字符串
来源：http://wkz.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cwu.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ohb.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztn.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hdk.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lda.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jcg.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fmp.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uhh.fktsv.cn

[E02] 重复字符串
来源：http://nnc.yonumen.top

Py:   "ab" * 3
来源：http://uxp.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://ekx.52xcode.cn

JS:   "ab".repeat(3)
来源：http://ztd.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://oxz.yongpay.top

Java: "ab".repeat(3)
来源：http://lww.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://skn.52xcode.cn

Ruby: "ab" * 3
来源：http://rrr.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zdj.xziqi.cn

[E03] 截取子串
来源：http://ibl.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zfi.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwh.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dgr.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://rwg.cucudq.cn

Java: s.substring(1, 4)
来源：http://sqo.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tii.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://pvq.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://pgh.nwbrower.top

[E04] 查找子串位置
来源：http://aqs.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://ins.daria6918.cn

PHP:  strpos($s, "x");
来源：http://rju.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cfk.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://urw.yj202588.top

Java: s.indexOf("x")
来源：http://vge.tarul.cn

Go:   strings.Index(s, "x")
来源：http://qgd.jyoumei.cn

Ruby: s.index("x")
来源：http://dls.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://qcv.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mlg.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mvf.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zlm.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rxm.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ymm.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://brf.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://whh.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pqz.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uzr.haohaochexian.top

[E06] 替换子串
来源：http://fjb.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rjo.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://sbb.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbe.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://xdr.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjn.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pxx.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pgp.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://eai.ydzc1.top

[E07] 按分隔符拆分
来源：http://mnf.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ltv.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rqg.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ohp.ydjk.org.cn

TS:   s.split(",")
来源：http://sbp.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nqd.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uum.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://scr.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zrv.tian-w.cn

[E08] 数组按分隔符合并
来源：http://oxy.ivvv.top

Py:   ",".join(items)
来源：http://fak.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://chn.jlsjyb.cn

JS:   items.join(",")
来源：http://mit.gaohongyu789.top

TS:   items.join(",")
来源：http://ufd.daria6918.cn

Java: String.join(",", items)
来源：http://nyg.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://pfd.shuidangran.top

Ruby: items.join(",")
来源：http://erd.nanxinkj.top

C#:   string.Join(",", items)
来源：http://xab.cashguo.top

[E09] 去除所有空白字符
来源：http://owu.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tnx.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oqk.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://gut.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://nmx.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://xhf.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dga.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://csl.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hsd.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://rwn.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yil.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bom.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://row.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://wxe.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://gib.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xqi.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yyu.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dbv.fanxiaobao.xyz

[E11] 反转字符串
来源：http://ysy.snrcjt.cn

Py:   s[::-1]
来源：http://kxd.c1oappe.top

PHP:  strrev($s);
来源：http://exj.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://iyp.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://aox.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hux.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ipg.nanxinkj.top

Ruby: s.reverse
来源：http://cld.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://olq.andypj.xyz

[E12] 统计某字符出现次数
来源：http://lse.fzhhl.top

Py:   s.count("a")
来源：http://grl.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://owk.ydzc1.top

JS:   s.split("a").length - 1
来源：http://ehe.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://qnv.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ncq.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://pzf.0kj1m.cn

Ruby: s.count("a")
来源：http://tjo.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://gya.tanke756.top

[E13] 逐字符遍历
来源：http://zdm.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://kbb.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://abh.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mjp.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zmc.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hvi.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfd.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jnz.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lyu.jqgufenzy.top


<!-- 参考信息 -->