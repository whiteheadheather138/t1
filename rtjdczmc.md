代发 wailian999

PHP:  sort($arr);
来源：http://vob.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wtl.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lox.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ocu.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jab.dianchejie.cn

Ruby: arr.sort
来源：http://tva.birdmap.top

C#:   list.Sort();
来源：http://xpd.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wyy.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jpt.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcq.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ysk.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nyf.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iph.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://flt.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rys.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jcl.pengpengdd.cyou

[D11] 反转数组
来源：http://exl.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ayj.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://gch.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://emz.sufxvd.cn

TS:   [...arr].reverse();
来源：http://oaq.ehwqpu.com

Java: Collections.reverse(list);
来源：http://mze.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://gia.bbcook.cn

Ruby: arr.reverse
来源：http://ygj.shzxlz.cn

C#:   list.Reverse();
来源：http://rpt.chenlongwang.top

[D12] 查找元素下标
来源：http://dgq.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://rti.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rjz.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xmk.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwb.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aap.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://hka.dashuyun.cn

Ruby: arr.index(x)
来源：http://asl.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://wxy.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://qlt.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://koc.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tlw.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://vzn.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://mkm.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xmn.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fjl.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zjk.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ble.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://opg.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ekn.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xpi.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://fjp.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://ssy.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pll.jqgufenzy.top

Go:   // 手写循环
来源：http://onv.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://see.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hnb.sysykeji.top

[D15] 去重
来源：http://zty.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qkf.shzxlz.cn

PHP:  array_unique($arr);
来源：http://kur.sweek.top

JS:   [...new Set(arr)]
来源：http://mnz.iojbl.cn

TS:   [...new Set(arr)]
来源：http://iao.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wvj.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://zrb.tarul.cn

Ruby: arr.uniq
来源：http://zog.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://flw.cdnleiting.top

[D16] 求和与平均值
来源：http://kux.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fik.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://viv.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwz.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqp.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dhl.epnwcf.com

Go:   // 手写循环累加
来源：http://ute.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wms.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://aak.hnqzz.top

[D17] 最大值与最小值
来源：http://xkc.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://tbb.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://alh.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ids.cqqwz.cn

TS:   Math.max(...arr);
来源：http://wgc.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ltf.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://olv.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://wis.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://aqj.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://njo.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nrg.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://vyt.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pyv.jlsjyb.cn

TS:   nested.flat();
来源：http://fbj.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wyo.yanxiufei.cn

Go:   // 手写双层循环
来源：http://zsk.zhongyouzk.top

Ruby: nested.flatten
来源：http://mgu.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hki.nanxuanxn.top

[D19] 按字段分组
来源：http://ofl.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pys.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dix.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pbd.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://egz.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tun.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://nhi.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://unt.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oex.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://grx.zhongyouzk.top

Py:   Counter(arr)
来源：http://hjj.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://wkh.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jhx.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vdi.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eis.daxiang520.top

Go:   // 手写 map[T]int
来源：http://els.fengsongda.top

Ruby: arr.tally
来源：http://qym.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eut.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://rod.gotoacloud.top

Py:   x in arr
来源：http://axu.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://zdx.bjfxy.top

JS:   arr.includes(x)
来源：http://bti.bbcook.cn

TS:   arr.includes(x)
来源：http://mvo.ppjwa.cn

Java: list.contains(x)
来源：http://mzs.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://vhi.yj20258888.top

Ruby: arr.include?(x)
来源：http://daj.zycfv.cn

C#:   list.Contains(x)
来源：http://api.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://xbf.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jzl.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ynw.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rvo.quarkkingdee.top

TS:   [...arr];
来源：http://dlo.xuanzx.com

Java: new ArrayList<>(list);
来源：http://kyp.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://lbp.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://xhc.zhijiandao.cn

C#:   new List<int>(list);
来源：http://waw.cashguo.top

[D23] reduce 累积计算
来源：http://ohb.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://odk.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://umj.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vqa.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hsd.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ffi.zhoulong.xyz

Go:   // 手写循环
来源：http://evc.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://otc.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iin.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://vzm.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://btx.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dfp.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pbx.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pxb.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ivu.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ifs.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bxy.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://paa.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://nyk.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ezc.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://khp.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyv.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zos.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ayf.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgm.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mcy.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ciz.nanxinkj.top

[D26] 数组转字符串
来源：http://oxv.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://kqq.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://yvn.zhijiandao.cn

JS:   arr.join(", ")
来源：http://okm.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://pqe.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://awh.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://dux.smart0.xyz

Ruby: arr.join(", ")
来源：http://qyb.ybcxt.top

C#:   string.Join(", ", list)
来源：http://exh.fzhhl.top

================================================================================
来源：http://ghv.ppjwa.cn

E. 字符串处理
来源：http://whf.zhoulong.xyz

================================================================================
来源：http://ujs.redwolf501.top

[E01] 拼接字符串
来源：http://alv.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vyj.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqd.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tjo.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://alw.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://egu.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mou.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nvs.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pub.52xcode.cn

[E02] 重复字符串
来源：http://zzr.vehdjk.com

Py:   "ab" * 3
来源：http://frz.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://qdu.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://fjq.jianghu66.top

TS:   "ab".repeat(3)
来源：http://abd.jiagoushi.top

Java: "ab".repeat(3)
来源：http://ahh.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://gpz.cqqwz.cn

Ruby: "ab" * 3
来源：http://ltz.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dil.zhongyouzk.top

[E03] 截取子串
来源：http://man.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qyw.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uql.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ull.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://yyx.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://nmz.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dbb.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yhp.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://ifj.yongpay.top

[E04] 查找子串位置
来源：http://sce.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://vqn.yuxming.cn

PHP:  strpos($s, "x");
来源：http://yet.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dvu.zhengqikj.top

TS:   s.indexOf("x")
来源：http://jaq.dianchejie.cn

Java: s.indexOf("x")
来源：http://ryy.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://jzy.birdmap.top

Ruby: s.index("x")
来源：http://xmm.xinyue.icu

C#:   s.IndexOf("x")
来源：http://tro.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wiz.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mao.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pfv.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hcu.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://djn.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qad.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uig.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fig.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eyp.xuanzx.com

[E06] 替换子串
来源：http://fxf.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kxl.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://wfa.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mpn.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://ekm.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psr.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sfh.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fmw.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://pbl.chenzaomai.com

[E07] 按分隔符拆分
来源：http://zkn.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pcu.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kwk.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fic.zhiwuduotai.top

TS:   s.split(",")
来源：http://lrl.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://fgz.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ist.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://zdm.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lts.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://mzf.havefunace.top

Py:   ",".join(items)
来源：http://yde.tanke756.top

PHP:  implode(",", $items);
来源：http://spf.gzhubu.top

JS:   items.join(",")
来源：http://sma.cdnleiting.top

TS:   items.join(",")
来源：http://cwt.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://xts.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://fmh.jqgfzy.top

Ruby: items.join(",")
来源：http://xel.sweek.top

C#:   string.Join(",", items)
来源：http://rcc.cqqwz.cn

[E09] 去除所有空白字符
来源：http://zdn.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldl.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yma.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://qcr.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://fdc.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://cyn.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wrk.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ego.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vtr.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://dcj.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fjn.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zxw.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://hqr.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://xaj.fktsv.cn

Java: String.format("%03d", 7)
来源：http://vpe.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mcw.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lan.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://arn.cheryme.top

[E11] 反转字符串
来源：http://zwk.hongshengwenyu.top

Py:   s[::-1]
来源：http://tbx.zhoulong.xyz

PHP:  strrev($s);
来源：http://glm.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://nsb.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://wyc.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ibx.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://phg.ydjk.org.cn

Ruby: s.reverse
来源：http://mrv.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://rdn.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://pga.aizwys.cn

Py:   s.count("a")
来源：http://foo.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://hau.bjfxy.top

JS:   s.split("a").length - 1
来源：http://qvw.andypj.xyz

TS:   s.split("a").length - 1
来源：http://mcv.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pqj.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://cpe.316326.xyz

Ruby: s.count("a")
来源：http://unm.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://ifx.mhx1999.top

[E13] 逐字符遍历
来源：http://hdm.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://gwh.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfa.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nda.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dwv.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mop.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mak.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mct.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tau.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://eko.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nvh.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dhq.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ynx.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cuc.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://css.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yph.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cvf.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dou.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://hxm.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hyz.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gbi.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://phk.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ioy.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://asx.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zjv.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tqi.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rnl.jiagoushi.top

[E16] 数字千分位
来源：http://jdu.yj20258888.top

Py:   f"{1234567:,}"
来源：http://daw.birdmap.top


<!-- 参考信息 -->