代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nqw.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qqg.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aqo.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qoy.jianghu66.top

[D11] 反转数组
来源：http://avh.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jio.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://ajb.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kan.zdqjudy.top

TS:   [...arr].reverse();
来源：http://qql.pycfn.com

Java: Collections.reverse(list);
来源：http://aag.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://tpw.ybcxt.top

Ruby: arr.reverse
来源：http://sgs.ydzc1.top

C#:   list.Reverse();
来源：http://tqf.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://msh.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://isc.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jib.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oew.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tuz.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sid.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://nhp.gaohongyu789.top

Ruby: arr.index(x)
来源：http://nra.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://wqv.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://lke.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ysc.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rnu.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://kif.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://mqf.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://guo.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fsm.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ige.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oyk.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://pdj.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://utk.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vua.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://hve.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://nmw.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jpt.haohaochexian.top

Go:   // 手写循环
来源：http://ehq.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ajr.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lor.redwolf501.top

[D15] 去重
来源：http://qcn.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cmz.9152youxi.cn

PHP:  array_unique($arr);
来源：http://pzb.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://czf.bbcook.cn

TS:   [...new Set(arr)]
来源：http://hic.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsw.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://yws.tian-w.cn

Ruby: arr.uniq
来源：http://zeb.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://znz.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://kkg.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uan.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nmu.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tjp.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwi.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://exk.nanxuanxn.top

Go:   // 手写循环累加
来源：http://mlm.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mkp.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://trr.tianlin.xyz

[D17] 最大值与最小值
来源：http://blj.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://ood.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://qut.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zgu.yvedp.cn

TS:   Math.max(...arr);
来源：http://uyv.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kwb.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rcr.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://ifm.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://qgs.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://sar.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rzv.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://hxl.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://djv.bbcook.cn

TS:   nested.flat();
来源：http://eqf.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://amt.uphjek.com

Go:   // 手写双层循环
来源：http://ggy.gogol.net.cn

Ruby: nested.flatten
来源：http://gfl.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ovu.zhiwuduotai.top

[D19] 按字段分组
来源：http://fuf.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kom.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gfn.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wbz.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wfq.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ojr.tanke756.top

Go:   // 手写 map[string][]T
来源：http://tkq.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xrf.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nih.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://nlj.zhongyouzk.top

Py:   Counter(arr)
来源：http://vgc.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://zpi.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ucp.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzw.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://det.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://ebw.daria6918.cn

Ruby: arr.tally
来源：http://zse.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qeb.ydzc1.top

[D21] 判断是否包含某元素
来源：http://vgn.zhixingplan.top

Py:   x in arr
来源：http://crh.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://gcd.yvedp.cn

JS:   arr.includes(x)
来源：http://jjk.daria6918.cn

TS:   arr.includes(x)
来源：http://izt.dianchejie.cn

Java: list.contains(x)
来源：http://iqj.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://opx.smart0.xyz

Ruby: arr.include?(x)
来源：http://agn.chenzaomai.com

C#:   list.Contains(x)
来源：http://juv.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://jdi.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwj.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bpy.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sxk.quarkkingdee.top

TS:   [...arr];
来源：http://trc.shuidangran.top

Java: new ArrayList<>(list);
来源：http://szw.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://mvt.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://esw.gzhubu.top

C#:   new List<int>(list);
来源：http://spx.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://zli.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mvm.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dta.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvv.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjs.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dve.gaohongyu789.top

Go:   // 手写循环
来源：http://ntg.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vxx.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsw.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://yxz.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rkx.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cto.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tey.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qdg.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ucf.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qpp.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pla.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://svf.316326.xyz

[D25] Set 集合去重与交并差
来源：http://uvf.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://poj.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lxc.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wvm.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jil.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sbi.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yui.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mst.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wks.yangfankeji.com

[D26] 数组转字符串
来源：http://fsp.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://fge.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://wkf.ivvv.top

JS:   arr.join(", ")
来源：http://qjz.iojbl.cn

TS:   arr.join(", ")
来源：http://xca.yuxming.cn

Java: String.join(", ", list)
来源：http://jfr.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://rfq.cashguo.top

Ruby: arr.join(", ")
来源：http://byk.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://mkb.meibo888.top

================================================================================
来源：http://vos.feifeiyinyue.top

E. 字符串处理
来源：http://waz.yuanzhike.top

================================================================================
来源：http://fqt.zycfv.cn

[E01] 拼接字符串
来源：http://doh.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yev.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vgo.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pka.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yov.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pkr.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mzk.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kxz.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jtu.9152youxi.cn

[E02] 重复字符串
来源：http://gam.ybcxt.top

Py:   "ab" * 3
来源：http://cks.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://vfi.316326.xyz

JS:   "ab".repeat(3)
来源：http://bhl.meibo888.top

TS:   "ab".repeat(3)
来源：http://fxz.yueranfly.top

Java: "ab".repeat(3)
来源：http://onf.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://dll.aibaodan.cn

Ruby: "ab" * 3
来源：http://zhk.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ugn.chenzaomai.com

[E03] 截取子串
来源：http://yvx.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hxv.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zwd.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ugr.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://fuv.svipenyu.cn

Java: s.substring(1, 4)
来源：http://nqu.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hov.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ymc.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://wgl.andypj.xyz

[E04] 查找子串位置
来源：http://reu.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://hzv.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://oig.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://red.nwbrower.top

TS:   s.indexOf("x")
来源：http://dxa.ivvv.top

Java: s.indexOf("x")
来源：http://vdv.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://lcz.haohaochexian.top

Ruby: s.index("x")
来源：http://glj.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://jiz.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://esx.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tfs.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zqr.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://klc.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://etj.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://omz.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uag.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vqg.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jlr.yangfankeji.com

[E06] 替换子串
来源：http://dvu.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://grc.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://msh.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjq.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://pje.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgq.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://poq.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uqo.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://pew.zdqjudy.top

[E07] 按分隔符拆分
来源：http://rkv.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ndl.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blb.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://abq.xuanzx.com

TS:   s.split(",")
来源：http://psi.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://ftb.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ofm.yongpay.top

Ruby: s.split(",");  s.split
来源：http://njq.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lfo.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://jvj.yongpay.top

Py:   ",".join(items)
来源：http://vfi.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://dcb.jqgfzy.top

JS:   items.join(",")
来源：http://dko.guannengcc.top

TS:   items.join(",")
来源：http://zsf.tianlin.xyz

Java: String.join(",", items)
来源：http://xnm.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://rcp.jqgfzy.top

Ruby: items.join(",")
来源：http://wmf.yonumen.top

C#:   string.Join(",", items)
来源：http://riu.aibaodan.cn

[E09] 去除所有空白字符
来源：http://qyj.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nxx.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nvc.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://qmb.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://rta.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://xda.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uto.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://xzx.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hrr.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://gul.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qjw.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qus.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://qvp.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://kiq.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://ekw.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://nio.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://euc.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jjb.yangfankeji.com

[E11] 反转字符串
来源：http://rcc.xuetiantiany.cn

Py:   s[::-1]
来源：http://qnd.shangyingyoupin.top

PHP:  strrev($s);
来源：http://tpp.yj20258.top

JS:   [...s].reverse().join("")
来源：http://ddq.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://exe.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://njo.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ums.iojbl.cn

Ruby: s.reverse
来源：http://wrm.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://fzk.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://kon.jinqigufen.top

Py:   s.count("a")
来源：http://tbk.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://jrd.yueranfly.top

JS:   s.split("a").length - 1
来源：http://whl.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://jni.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fzg.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://bmv.chenzaomai.com

Ruby: s.count("a")
来源：http://pij.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://nbf.xinyue.icu

[E13] 逐字符遍历
来源：http://gkt.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://afr.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vjz.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fei.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://adx.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eoj.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uyy.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iwg.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xmu.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://zve.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mko.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wbc.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://txb.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vrz.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vdy.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ail.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wrh.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vmd.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://zts.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mnd.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dna.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vxf.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ope.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfo.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bod.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jgz.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tty.yj202588.top

[E16] 数字千分位
来源：http://hsp.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://gar.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://piu.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://weu.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yvw.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xml.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xru.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ntg.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://zra.uphjek.com

[E17] 首字母大写
来源：http://qyi.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zmt.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kpl.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gzg.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mvm.zhongyouzk.top


<!-- 参考信息 -->