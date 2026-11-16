代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lqi.yangfankeji.com

Ruby: arr.sort
来源：http://ogx.uphjek.com

C#:   list.Sort();
来源：http://fqc.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kyd.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qlu.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lrd.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbn.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mya.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zur.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hww.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eyj.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://esz.bjfxy.top

[D11] 反转数组
来源：http://xgb.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://afc.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://lnv.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjn.zdbjq.cn

TS:   [...arr].reverse();
来源：http://lgy.sweek.top

Java: Collections.reverse(list);
来源：http://fuz.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://cku.chenjidiqi.icu

Ruby: arr.reverse
来源：http://bfm.daria6918.cn

C#:   list.Reverse();
来源：http://fge.jqgfzy.top

[D12] 查找元素下标
来源：http://cct.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://xul.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yze.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://udt.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xqa.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pkn.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://ibx.9152youxi.cn

Ruby: arr.index(x)
来源：http://hbh.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://udg.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://qyx.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lso.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mil.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://nmg.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://sgl.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://knm.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nye.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://rbg.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gbb.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://vea.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://may.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vxn.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://ksm.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://iuc.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xnw.ctjpmb.com

Go:   // 手写循环
来源：http://htp.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://naw.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rij.tianlin.xyz

[D15] 去重
来源：http://jmp.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://erc.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://ffv.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://gtr.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://fpp.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nps.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://sga.shangyingyoupin.top

Ruby: arr.uniq
来源：http://jci.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://ory.meibo888.top

[D16] 求和与平均值
来源：http://qfl.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://typ.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hug.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://adv.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zgc.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ubd.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://jbd.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nzc.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://fza.yj202588.top

[D17] 最大值与最小值
来源：http://vwr.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://diz.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://nfv.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kzo.yuxming.cn

TS:   Math.max(...arr);
来源：http://fhy.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jle.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://euf.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://rqy.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://xec.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://tqj.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nej.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://tpe.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dqm.feifeiyinyue.top

TS:   nested.flat();
来源：http://tqf.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ges.gogol.net.cn

Go:   // 手写双层循环
来源：http://rsp.316326.xyz

Ruby: nested.flatten
来源：http://grf.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kft.xuetiantiany.cn

[D19] 按字段分组
来源：http://qwf.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yvo.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://asf.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hdu.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sxu.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwb.yonumen.top

Go:   // 手写 map[string][]T
来源：http://aoc.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ury.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xmb.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://pcz.tianlin.xyz

Py:   Counter(arr)
来源：http://yey.epnwcf.com

PHP:  array_count_values($arr);
来源：http://pxa.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fun.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dre.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://unr.fehbvm.com

Go:   // 手写 map[T]int
来源：http://hgy.daxiang520.top

Ruby: arr.tally
来源：http://hbd.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aeo.uphjek.com

[D21] 判断是否包含某元素
来源：http://jea.yj20258888.top

Py:   x in arr
来源：http://zvj.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://pmk.hnxiangtu.top

JS:   arr.includes(x)
来源：http://buo.hcnkem.com

TS:   arr.includes(x)
来源：http://yyt.chenlongwang.top

Java: list.contains(x)
来源：http://eww.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://uab.zycfv.cn

Ruby: arr.include?(x)
来源：http://cqa.daxiang520.top

C#:   list.Contains(x)
来源：http://dvk.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://ptl.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dcv.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://avr.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ath.cheryme.top

TS:   [...arr];
来源：http://dpp.fehbvm.com

Java: new ArrayList<>(list);
来源：http://kof.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://kpc.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://fky.zhijiandao.cn

C#:   new List<int>(list);
来源：http://lsr.haohaochexian.top

[D23] reduce 累积计算
来源：http://yjh.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zbj.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nzc.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rvw.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ade.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gaq.9152youxi.cn

Go:   // 手写循环
来源：http://mjr.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qzl.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xer.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://mih.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rpl.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jml.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://awp.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wqz.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wuu.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eof.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nqe.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ekk.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://enq.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bcn.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dpl.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ium.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ple.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gcm.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ibb.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iwp.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ocn.cqqwz.cn

[D26] 数组转字符串
来源：http://lav.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://zlj.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://qva.zhongyouzk.top

JS:   arr.join(", ")
来源：http://ion.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://lck.9152youxi.cn

Java: String.join(", ", list)
来源：http://bej.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://axd.nanxinkj.top

Ruby: arr.join(", ")
来源：http://lxl.yongpay.top

C#:   string.Join(", ", list)
来源：http://abj.vehdjk.com

================================================================================
来源：http://tpd.shanyushiyangtech.top

E. 字符串处理
来源：http://akb.jyoumei.cn

================================================================================
来源：http://ssq.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://eme.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bii.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nix.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ivv.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jmh.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cam.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cvu.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hhr.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ivn.fzhhl.top

[E02] 重复字符串
来源：http://qfh.ydjk.org.cn

Py:   "ab" * 3
来源：http://uwa.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://kzt.smart0.xyz

JS:   "ab".repeat(3)
来源：http://jyt.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://srz.haohaochexian.top

Java: "ab".repeat(3)
来源：http://ozf.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://faf.0kj1m.cn

Ruby: "ab" * 3
来源：http://fwp.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bis.bjfxy.top

[E03] 截取子串
来源：http://beh.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://net.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gft.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rzn.cashguo.top

TS:   s.slice(1, 4)
来源：http://jna.ybcxt.top

Java: s.substring(1, 4)
来源：http://qvs.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xqx.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://roy.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://jku.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://qeq.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://len.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://dvc.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wyd.sufxvd.cn

TS:   s.indexOf("x")
来源：http://sux.52xcode.cn

Java: s.indexOf("x")
来源：http://qsp.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://lzz.zhoulong.xyz

Ruby: s.index("x")
来源：http://riv.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://tgy.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://goi.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yyc.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gsw.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyq.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kku.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyh.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bxk.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgk.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qso.feifeiyinyue.top

[E06] 替换子串
来源：http://qch.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cpc.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://jbo.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wls.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://lvq.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xre.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bgy.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://snv.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://jdj.yangfankeji.com

[E07] 按分隔符拆分
来源：http://tpr.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wvn.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://whc.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sae.quarkkingdee.top

TS:   s.split(",")
来源：http://uel.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uer.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oas.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://qra.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eho.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://nto.kuanghao11.cn

Py:   ",".join(items)
来源：http://azl.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://esn.ivvv.top

JS:   items.join(",")
来源：http://uqf.aibaodan.cn

TS:   items.join(",")
来源：http://ppw.wangshuangyany.cn

Java: String.join(",", items)
来源：http://cvm.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://knx.zhengqikj.top

Ruby: items.join(",")
来源：http://ngs.xylfe.cn

C#:   string.Join(",", items)
来源：http://lrl.fengsongda.top

[E09] 去除所有空白字符
来源：http://ipz.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bam.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cho.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://ehh.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://ito.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://nio.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hqa.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://cjs.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vnn.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://ojj.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jxf.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kwt.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://bqq.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://nqi.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://vwm.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fsc.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lyr.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oau.zhixingplan.top

[E11] 反转字符串
来源：http://ywe.jinghuilouyu.cn

Py:   s[::-1]
来源：http://yeo.nanxinkj.top

PHP:  strrev($s);
来源：http://gvf.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://gqf.pycfn.com

TS:   [...s].reverse().join("")
来源：http://iqs.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hte.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://txs.jiagoushi.top

Ruby: s.reverse
来源：http://lvf.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://prp.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://xlq.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://omx.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://dlz.fengsongda.top

JS:   s.split("a").length - 1
来源：http://yje.wangdashe.top

TS:   s.split("a").length - 1
来源：http://tqj.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jmy.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://yuh.quarkkingdee.top

Ruby: s.count("a")
来源：http://suw.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://dym.sweek.top

[E13] 逐字符遍历
来源：http://keb.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://cvw.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kin.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xuh.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mqb.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ftw.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aef.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ymu.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ovv.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://acb.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yfv.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lbv.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://awp.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yfp.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jfi.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mix.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eou.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cjd.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://wlp.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rtr.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vlg.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tze.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://nyj.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbm.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yjn.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xrn.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yvw.sxryk.cn

[E16] 数字千分位
来源：http://vkc.52xcode.cn

Py:   f"{1234567:,}"
来源：http://pyn.yonumen.top

PHP:  number_format(1234567);
来源：http://agl.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gav.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://jht.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cyw.vehdjk.com


<!-- 参考信息 -->