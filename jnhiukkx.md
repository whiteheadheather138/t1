代发 wailian999

PHP:  sort($arr);
来源：http://atx.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qew.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://erh.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mpd.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fut.fktsv.cn

Ruby: arr.sort
来源：http://chl.sufxvd.cn

C#:   list.Sort();
来源：http://mjx.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kdo.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ahd.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejf.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://roi.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wde.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bxk.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zta.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vyo.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mgk.zhijiandao.cn

[D11] 反转数组
来源：http://blv.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://sgw.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://fiv.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tvq.ivvv.top

TS:   [...arr].reverse();
来源：http://xky.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://etz.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://ewb.xziqi.cn

Ruby: arr.reverse
来源：http://rcn.sweek.top

C#:   list.Reverse();
来源：http://blh.zhengqikj.top

[D12] 查找元素下标
来源：http://dlg.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://dls.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hwj.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ncp.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhr.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ezz.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://ksl.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://pht.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://bsp.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://wdx.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://akh.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jqd.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://vwf.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://bic.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbu.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rct.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://hlv.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eeh.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://kqc.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://org.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hah.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://jmq.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://qof.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qsy.jiagoushi.top

Go:   // 手写循环
来源：http://zyk.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yae.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://egm.ppjwa.cn

[D15] 去重
来源：http://hfz.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uax.redwolf501.top

PHP:  array_unique($arr);
来源：http://omj.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://hri.yj202588.top

TS:   [...new Set(arr)]
来源：http://vka.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yoj.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ptx.zdqjudy.top

Ruby: arr.uniq
来源：http://wwr.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://hvz.andypj.xyz

[D16] 求和与平均值
来源：http://iqh.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pjb.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vvk.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bng.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpn.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hug.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://qoz.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xtc.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://amw.dianchejie.cn

[D17] 最大值与最小值
来源：http://uil.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://eqr.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://ynd.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://has.zhixingplan.top

TS:   Math.max(...arr);
来源：http://awd.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vsm.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jfa.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://iwg.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://sex.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://cxg.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eqb.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://wto.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ppu.bjfxy.top

TS:   nested.flat();
来源：http://lbo.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fbu.zycfv.cn

Go:   // 手写双层循环
来源：http://jdi.hongshengwenyu.top

Ruby: nested.flatten
来源：http://tls.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pxo.xylfe.cn

[D19] 按字段分组
来源：http://odj.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cfr.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kfl.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oya.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jne.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lkf.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://zkg.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mkf.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ckt.yongpay.top

[D20] 统计每个元素出现次数
来源：http://zgy.zhixingplan.top

Py:   Counter(arr)
来源：http://nca.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://pgb.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gip.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnq.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fjr.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://iux.hammf.cn

Ruby: arr.tally
来源：http://nqw.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tbg.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://dwf.hysaishi.cn

Py:   x in arr
来源：http://rcv.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://vqt.yvedp.cn

JS:   arr.includes(x)
来源：http://yxg.meibo888.top

TS:   arr.includes(x)
来源：http://vlv.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://uwx.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://kqc.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://gxl.yangfankeji.com

C#:   list.Contains(x)
来源：http://lla.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://oug.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iru.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iks.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mwe.hcnkem.com

TS:   [...arr];
来源：http://rfl.yongpay.top

Java: new ArrayList<>(list);
来源：http://shs.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://cor.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://hgi.jlsjyb.cn

C#:   new List<int>(list);
来源：http://ipe.andypj.xyz

[D23] reduce 累积计算
来源：http://tmk.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://okp.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://otf.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsk.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eee.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rkl.mhx1999.top

Go:   // 手写循环
来源：http://yhl.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fdy.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ylt.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://pwm.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vsh.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gxi.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://umq.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ufn.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tdt.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vvq.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mqr.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qwq.sweek.top

[D25] Set 集合去重与交并差
来源：http://pfo.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ypd.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kxj.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://olk.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ckk.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwk.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://acz.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mjy.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qtw.redwolf501.top

[D26] 数组转字符串
来源：http://cdd.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://ylj.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://hug.ydjk.org.cn

JS:   arr.join(", ")
来源：http://obq.xinyue.icu

TS:   arr.join(", ")
来源：http://vse.xylfe.cn

Java: String.join(", ", list)
来源：http://ekh.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://res.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://ezj.yvedp.cn

C#:   string.Join(", ", list)
来源：http://sus.daxiang520.top

================================================================================
来源：http://bds.bjfxy.top

E. 字符串处理
来源：http://mka.daxiang520.top

================================================================================
来源：http://ylg.guowangkeji.top

[E01] 拼接字符串
来源：http://yhr.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pns.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mcg.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ijh.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xum.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nrs.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://prr.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ksm.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jir.ybcxt.top

[E02] 重复字符串
来源：http://qax.hywenlv.cn

Py:   "ab" * 3
来源：http://sxg.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://pjn.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://rlg.aizwys.cn

TS:   "ab".repeat(3)
来源：http://lds.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://jjw.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://gzp.ctjpmb.com

Ruby: "ab" * 3
来源：http://oet.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bwr.vqdsnc.cn

[E03] 截取子串
来源：http://ohi.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rtz.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wtg.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hme.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://fxn.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://rpe.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ghi.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://emu.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://khf.yonumen.top

[E04] 查找子串位置
来源：http://eyi.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://jxu.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://cwb.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nvq.sysykeji.top

TS:   s.indexOf("x")
来源：http://mah.aizwys.cn

Java: s.indexOf("x")
来源：http://akt.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://nfl.hongshengwenyu.top

Ruby: s.index("x")
来源：http://bxt.yj20258.top

C#:   s.IndexOf("x")
来源：http://uew.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kya.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcp.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owr.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgr.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uds.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrp.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ula.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvz.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fgi.zhoulong.xyz

[E06] 替换子串
来源：http://csc.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://snk.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://ffd.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bpe.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://ixx.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhh.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lpo.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hbp.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://nie.hysaishi.cn

[E07] 按分隔符拆分
来源：http://gkg.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jks.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zcf.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rmj.gotoacloud.top

TS:   s.split(",")
来源：http://qll.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://yli.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://axv.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://gvv.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qud.fehbvm.com

[E08] 数组按分隔符合并
来源：http://pcp.jianghu66.top

Py:   ",".join(items)
来源：http://mnj.fehbvm.com

PHP:  implode(",", $items);
来源：http://upw.zhijiandao.cn

JS:   items.join(",")
来源：http://tzi.wangshuangyany.cn

TS:   items.join(",")
来源：http://vym.sysykeji.top

Java: String.join(",", items)
来源：http://bmy.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://xyu.vehdjk.com

Ruby: items.join(",")
来源：http://eru.birdmap.top

C#:   string.Join(",", items)
来源：http://jiq.vehdjk.com

[E09] 去除所有空白字符
来源：http://zqs.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pnr.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bfw.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://lwr.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://mun.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://oqr.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ild.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iqa.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://thk.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://irx.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kqz.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rks.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://cux.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://uho.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://iyh.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rry.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kwx.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gsc.vehdjk.com

[E11] 反转字符串
来源：http://jqq.nanxuanxn.top

Py:   s[::-1]
来源：http://rlc.quarkkingdee.top

PHP:  strrev($s);
来源：http://mcr.ivvv.top

JS:   [...s].reverse().join("")
来源：http://lyz.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://qik.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xei.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://wei.gotoacloud.top

Ruby: s.reverse
来源：http://rgo.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://log.tian-w.cn

[E12] 统计某字符出现次数
来源：http://viw.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://dij.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://zjn.tian-w.cn

JS:   s.split("a").length - 1
来源：http://zsr.cheryme.top

TS:   s.split("a").length - 1
来源：http://ypp.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vcm.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://bld.pengpengdd.cyou

Ruby: s.count("a")
来源：http://hvi.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://qda.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://tmc.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://jyz.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://buh.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nna.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gos.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btd.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qmo.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://epk.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://imk.birdmap.top

[E14] URL 编码与 Base64
来源：http://lxu.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://twg.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bfe.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ifd.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nvk.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://itb.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wja.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mke.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://twg.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://rrn.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xdl.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eit.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jwe.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hsg.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lar.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ckq.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qwq.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kiu.jlsjyb.cn

[E16] 数字千分位
来源：http://cgg.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://wyi.epnwcf.com


<!-- 参考信息 -->