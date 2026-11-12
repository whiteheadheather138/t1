代发 wailian999

TS:   arr.slice(1, 4);
来源：http://dlt.xinyue.icu

Java: list.subList(1, 4);
来源：http://ajh.jiagoushi.top

Go:   arr[1:4]
来源：http://mpd.gzhubu.top

Ruby: arr[1, 3]
来源：http://irn.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://gtd.316326.xyz

[D08] 合并两个数组
来源：http://scl.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://rdn.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://bej.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fsp.havefunace.top

TS:   [...a, ...b];
来源：http://fbp.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://buy.zhiwuduotai.top

Go:   append(a, b...)
来源：http://oow.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://obv.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://nte.gzhubu.top

[D09] 排序（升序）
来源：http://zeu.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://xuc.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://fvb.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://von.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wdd.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kxk.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gxt.zycfv.cn

Ruby: arr.sort
来源：http://tln.ehwqpu.com

C#:   list.Sort();
来源：http://tap.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yii.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wzs.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xcu.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jsi.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://inh.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pjj.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dzg.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fqm.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lsr.xinyue.icu

[D11] 反转数组
来源：http://iyj.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://odu.hnqzz.top

PHP:  array_reverse($arr);
来源：http://xqe.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qae.guannengcc.top

TS:   [...arr].reverse();
来源：http://jea.nanxinkj.top

Java: Collections.reverse(list);
来源：http://ewo.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://fav.mhx1999.top

Ruby: arr.reverse
来源：http://qwh.tarul.cn

C#:   list.Reverse();
来源：http://mph.jinqigfzy.top

[D12] 查找元素下标
来源：http://ssd.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://bpp.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ytf.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdt.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uer.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jcg.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://jim.yj20258.top

Ruby: arr.index(x)
来源：http://jik.fzhhl.top

C#:   list.IndexOf(x);
来源：http://dcf.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://squ.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xyl.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zqu.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://mno.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://xux.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ieu.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zgh.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://bpe.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://smw.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://ejb.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://weq.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hwo.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://cea.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://kgb.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://wjo.meibo888.top

Go:   // 手写循环
来源：http://amb.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://tru.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wkm.jinqigufen.top

[D15] 去重
来源：http://pfu.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rrt.snrcjt.cn

PHP:  array_unique($arr);
来源：http://wxg.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://fpl.ybcxt.top

TS:   [...new Set(arr)]
来源：http://jms.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyc.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://etq.iojbl.cn

Ruby: arr.uniq
来源：http://agz.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://szx.jinqigfzy.top

[D16] 求和与平均值
来源：http://clq.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bcj.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vzd.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhd.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxf.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xar.nanxuanxn.top

Go:   // 手写循环累加
来源：http://the.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://geq.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://pgk.zhijiandao.cn

[D17] 最大值与最小值
来源：http://xfd.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://mjr.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://fji.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fcf.smart0.xyz

TS:   Math.max(...arr);
来源：http://juf.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vfs.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://awn.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://wya.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://phf.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://yep.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rfp.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://kyq.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lcj.wangdashe.top

TS:   nested.flat();
来源：http://emy.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jhr.mhx1999.top

Go:   // 手写双层循环
来源：http://wto.tian-w.cn

Ruby: nested.flatten
来源：http://gdt.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohl.gotoacloud.top

[D19] 按字段分组
来源：http://uwz.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xsc.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://doj.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aax.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qhp.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gsv.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://meh.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://otm.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mkt.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://ftb.meibo888.top

Py:   Counter(arr)
来源：http://fbx.vehdjk.com

PHP:  array_count_values($arr);
来源：http://jqm.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvh.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://att.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yol.shuidangran.top

Go:   // 手写 map[T]int
来源：http://tvb.fengsongda.top

Ruby: arr.tally
来源：http://kny.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://knh.yfazqb.com

[D21] 判断是否包含某元素
来源：http://kbs.wangdashe.top

Py:   x in arr
来源：http://vrp.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://lrh.ivvv.top

JS:   arr.includes(x)
来源：http://yzl.ybcxt.top

TS:   arr.includes(x)
来源：http://wfh.feifeiyinyue.top

Java: list.contains(x)
来源：http://hqr.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://bjy.uphjek.com

Ruby: arr.include?(x)
来源：http://xnr.ctjpmb.com

C#:   list.Contains(x)
来源：http://hws.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://gwi.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kta.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://css.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kue.sweek.top

TS:   [...arr];
来源：http://msr.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://aon.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://cmn.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://osr.yuanzhike.top

C#:   new List<int>(list);
来源：http://yob.yuanzhike.top

[D23] reduce 累积计算
来源：http://her.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lkx.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://igj.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xqa.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iax.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ssf.hcnkem.com

Go:   // 手写循环
来源：http://veo.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xof.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oss.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://nbr.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qlg.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ywa.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rfx.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://isb.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pny.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://clf.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://woc.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iwl.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://yza.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ptw.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://unl.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mww.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dks.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cye.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yst.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://evs.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dss.yangfankeji.com

[D26] 数组转字符串
来源：http://wtv.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://xdq.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://gbb.c1oappe.top

JS:   arr.join(", ")
来源：http://inx.birdmap.top

TS:   arr.join(", ")
来源：http://kch.aizwys.cn

Java: String.join(", ", list)
来源：http://wzn.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://dyl.gogol.net.cn

Ruby: arr.join(", ")
来源：http://ibj.hcnkem.com

C#:   string.Join(", ", list)
来源：http://jko.jyoumei.cn

================================================================================
来源：http://vkv.c1oappe.top

E. 字符串处理
来源：http://rop.shangyingyoupin.top

================================================================================
来源：http://bwo.hysaishi.cn

[E01] 拼接字符串
来源：http://cvn.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bwh.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cfk.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tpb.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybt.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://izn.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lfz.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwb.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlj.hywenlv.cn

[E02] 重复字符串
来源：http://pma.fehbvm.com

Py:   "ab" * 3
来源：http://aul.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://bef.sysykeji.top

JS:   "ab".repeat(3)
来源：http://fha.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://ymd.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://fdn.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://iwb.smart0.xyz

Ruby: "ab" * 3
来源：http://dlk.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rxn.hongshengwenyu.top

[E03] 截取子串
来源：http://yoz.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gsv.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lvw.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ggh.vehdjk.com

TS:   s.slice(1, 4)
来源：http://zne.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://adp.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bji.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hus.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://mre.tarul.cn

[E04] 查找子串位置
来源：http://ehr.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://pjp.zycfv.cn

PHP:  strpos($s, "x");
来源：http://fmh.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tlx.dashuyun.cn

TS:   s.indexOf("x")
来源：http://miu.nanxuanxn.top

Java: s.indexOf("x")
来源：http://jot.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://mbd.cdnleiting.top

Ruby: s.index("x")
来源：http://ipn.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://eds.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://khg.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ahr.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://thk.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://olb.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nvn.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rye.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://avk.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zjp.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eex.tianlin.xyz

[E06] 替换子串
来源：http://tid.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgt.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://hdz.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioo.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://pfl.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cku.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pzd.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://noc.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://nlt.ctjpmb.com

[E07] 按分隔符拆分
来源：http://frc.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tvt.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://okz.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iip.ctjpmb.com

TS:   s.split(",")
来源：http://vre.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://opa.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://teu.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://wto.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://djk.hesvh.cn

[E08] 数组按分隔符合并
来源：http://oeu.cheryme.top

Py:   ",".join(items)
来源：http://feh.pycfn.com

PHP:  implode(",", $items);
来源：http://rbl.jlsjyb.cn

JS:   items.join(",")
来源：http://mcf.birdmap.top

TS:   items.join(",")
来源：http://ckm.cucudq.cn

Java: String.join(",", items)
来源：http://osj.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://vsp.shzxlz.cn

Ruby: items.join(",")
来源：http://fol.sysykeji.top

C#:   string.Join(",", items)
来源：http://hmv.gogol.net.cn

[E09] 去除所有空白字符
来源：http://buh.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vsd.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kaj.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://qao.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://spz.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://omh.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qnl.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://dum.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ujt.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://nfa.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://acn.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hel.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://tvn.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://qmu.yfazqb.com

Java: String.format("%03d", 7)
来源：http://jws.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xpj.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ael.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://trh.ehwqpu.com

[E11] 反转字符串
来源：http://mqp.9152youxi.cn

Py:   s[::-1]
来源：http://dze.hywenlv.cn

PHP:  strrev($s);
来源：http://dvr.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://gif.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://zvf.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pzf.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://epc.zhiwuduotai.top

Ruby: s.reverse
来源：http://txh.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://yvc.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://jed.svipenyu.cn

Py:   s.count("a")
来源：http://wes.yj202588.top

PHP:  substr_count($s, "a");
来源：http://vav.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://nfv.hcnkem.com

TS:   s.split("a").length - 1
来源：http://xgm.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gwb.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://lyh.jinqigufen.top

Ruby: s.count("a")
来源：http://czk.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://wdy.yangfankeji.com

[E13] 逐字符遍历
来源：http://qfg.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://fbe.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ljz.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://qsi.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qye.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kiw.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zfl.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zld.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gtb.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://lmu.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qcr.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ran.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sod.hysaishi.cn


<!-- 参考信息 -->