代发 wailian999

PHP:  sort($arr);
来源：http://ovv.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tjq.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bnl.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fcf.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjg.nanxinkj.top

Ruby: arr.sort
来源：http://uyh.birdmap.top

C#:   list.Sort();
来源：http://atc.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jyt.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bii.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://okd.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfj.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://djl.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gnx.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qvm.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ycq.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fxd.yueranfly.top

[D11] 反转数组
来源：http://uxz.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://rwh.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://vzm.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lmh.sysykeji.top

TS:   [...arr].reverse();
来源：http://gzx.guannengcc.top

Java: Collections.reverse(list);
来源：http://iwa.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://rjw.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://ool.xylfe.cn

C#:   list.Reverse();
来源：http://qts.aibaodan.cn

[D12] 查找元素下标
来源：http://sov.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://kgd.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://phs.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kkb.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hbr.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lgq.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://ump.52xcode.cn

Ruby: arr.index(x)
来源：http://vci.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://kho.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://xkr.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bhr.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayc.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://flv.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://jcv.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ule.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hhd.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gdm.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dsi.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://aee.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xhx.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://djd.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://frx.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://caf.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aad.0kj1m.cn

Go:   // 手写循环
来源：http://gkr.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://mms.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jzb.tian-w.cn

[D15] 去重
来源：http://que.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bzd.redwolf501.top

PHP:  array_unique($arr);
来源：http://ybw.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://oac.yuxming.cn

TS:   [...new Set(arr)]
来源：http://owa.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ssm.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://slf.birdmap.top

Ruby: arr.uniq
来源：http://ime.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://pov.birdmap.top

[D16] 求和与平均值
来源：http://fqw.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lza.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://okv.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gnm.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afx.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ypb.sweek.top

Go:   // 手写循环累加
来源：http://ick.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bwg.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://cpo.ppjwa.cn

[D17] 最大值与最小值
来源：http://yhn.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://zjp.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://dcm.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cks.cqqwz.cn

TS:   Math.max(...arr);
来源：http://vot.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iqp.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yxp.tanke756.top

Ruby: arr.max;  arr.min
来源：http://pdj.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://eqb.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://zmf.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lmz.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://pkf.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ckq.smart0.xyz

TS:   nested.flat();
来源：http://vhq.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rkf.jinqigfzy.top

Go:   // 手写双层循环
来源：http://ref.jiagoushi.top

Ruby: nested.flatten
来源：http://cyd.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cqi.wangdashe.top

[D19] 按字段分组
来源：http://trl.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aoh.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbf.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://psa.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://azw.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wqk.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://nho.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://foq.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wzq.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://iij.zhoulong.xyz

Py:   Counter(arr)
来源：http://mzu.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://oon.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rso.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jjp.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uly.ybcxt.top

Go:   // 手写 map[T]int
来源：http://qav.zdqjudy.top

Ruby: arr.tally
来源：http://btg.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oss.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://nbd.zhiwuduotai.top

Py:   x in arr
来源：http://ooc.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://znf.dianchejie.cn

JS:   arr.includes(x)
来源：http://noz.cucudq.cn

TS:   arr.includes(x)
来源：http://jxo.yj202588.top

Java: list.contains(x)
来源：http://cmt.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://efg.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://qxu.fehbvm.com

C#:   list.Contains(x)
来源：http://dbc.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://zib.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xnr.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hrv.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uhh.sxryk.cn

TS:   [...arr];
来源：http://hkb.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://bkw.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://sip.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://ypk.sufxvd.cn

C#:   new List<int>(list);
来源：http://gun.yuxming.cn

[D23] reduce 累积计算
来源：http://egx.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zsq.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ocp.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rno.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pvk.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkb.iojbl.cn

Go:   // 手写循环
来源：http://cmn.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bge.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pgi.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://xgf.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://goo.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://elv.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://drf.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hdh.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ljo.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pab.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://asd.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://acw.meibo888.top

[D25] Set 集合去重与交并差
来源：http://qpm.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwn.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://icb.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dwe.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dav.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://drs.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zvt.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ivk.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qeb.zycfv.cn

[D26] 数组转字符串
来源：http://mxs.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://upd.meibo888.top

PHP:  implode(", ", $arr);
来源：http://uzq.daxiang520.top

JS:   arr.join(", ")
来源：http://psf.hywenlv.cn

TS:   arr.join(", ")
来源：http://iov.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://bre.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://jde.gzhubu.top

Ruby: arr.join(", ")
来源：http://qyk.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://mpf.aibaodan.cn

================================================================================
来源：http://dys.xuetiantiany.cn

E. 字符串处理
来源：http://hdx.meibo888.top

================================================================================
来源：http://kce.zhoulong.xyz

[E01] 拼接字符串
来源：http://ddj.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://alj.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fnb.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwo.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://neq.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jnd.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jxd.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qcj.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xux.daria6918.cn

[E02] 重复字符串
来源：http://dac.zycfv.cn

Py:   "ab" * 3
来源：http://utz.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://xdu.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://fxz.ybcxt.top

TS:   "ab".repeat(3)
来源：http://prt.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://qiq.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://hsl.gotoacloud.top

Ruby: "ab" * 3
来源：http://lur.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dru.nanxuanxn.top

[E03] 截取子串
来源：http://xwp.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rni.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pyb.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nqi.cashguo.top

TS:   s.slice(1, 4)
来源：http://hir.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://sft.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jef.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://jnd.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://lum.zdqjudy.top

[E04] 查找子串位置
来源：http://gjs.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://res.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://wxi.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://roi.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://xsd.redwolf501.top

Java: s.indexOf("x")
来源：http://wwd.havefunace.top

Go:   strings.Index(s, "x")
来源：http://pjq.snrcjt.cn

Ruby: s.index("x")
来源：http://oad.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://nnc.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lcb.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rlm.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mfa.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ihr.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ojx.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmo.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://neo.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oiz.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gox.jianghu66.top

[E06] 替换子串
来源：http://pyn.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pkm.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://jdy.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://itq.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://aon.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ups.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hcl.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://edm.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://icd.shuidangran.top

[E07] 按分隔符拆分
来源：http://pww.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ujd.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://die.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tet.yongpay.top

TS:   s.split(",")
来源：http://evs.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://lbv.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wic.tarul.cn

Ruby: s.split(",");  s.split
来源：http://hxy.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lyi.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://yxh.iojbl.cn

Py:   ",".join(items)
来源：http://tqw.hnqzz.top

PHP:  implode(",", $items);
来源：http://qqq.xziqi.cn

JS:   items.join(",")
来源：http://xxr.hnxiangtu.top

TS:   items.join(",")
来源：http://ejr.zhiwuduotai.top

Java: String.join(",", items)
来源：http://bkg.yj20258.top

Go:   strings.Join(items, ",")
来源：http://wqf.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://msr.gotoacloud.top

C#:   string.Join(",", items)
来源：http://qwl.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://zcj.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mzg.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qbm.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://ipu.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://izp.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://uip.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mli.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://khy.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dtl.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://yjb.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ist.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mcd.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://edz.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://qsm.cashguo.top

Java: String.format("%03d", 7)
来源：http://cvg.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rjg.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zkq.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yjw.xinyue.icu

[E11] 反转字符串
来源：http://hfp.quarkkingdee.top

Py:   s[::-1]
来源：http://iif.meibo888.top

PHP:  strrev($s);
来源：http://ipo.sweek.top

JS:   [...s].reverse().join("")
来源：http://kck.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://ckr.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://rny.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qlt.tianlin.xyz

Ruby: s.reverse
来源：http://ngj.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://ywx.hesvh.cn

[E12] 统计某字符出现次数
来源：http://tft.ctjpmb.com

Py:   s.count("a")
来源：http://fyb.316326.xyz

PHP:  substr_count($s, "a");
来源：http://cio.hnqzz.top

JS:   s.split("a").length - 1
来源：http://rpr.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://pyu.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdi.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://fai.wangshuangyany.cn

Ruby: s.count("a")
来源：http://jyo.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://clf.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://wlx.yj202588.top

Py:   for ch in s: print(ch)
来源：http://uiv.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ili.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xtz.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xes.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dpr.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hjm.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tki.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rar.uphjek.com

[E14] URL 编码与 Base64
来源：http://cwu.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xze.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cow.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lra.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qci.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://equ.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uzq.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://don.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qls.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://and.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://vlq.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pgu.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dud.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mbv.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fyj.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xqj.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwp.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://evs.0kj1m.cn

[E16] 数字千分位
来源：http://wtl.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://gmb.uphjek.com


<!-- 参考信息 -->