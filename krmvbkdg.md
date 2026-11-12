代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://jqd.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://aue.bbcook.cn

[D09] 排序（升序）
来源：http://bsb.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://utc.birdmap.top

PHP:  sort($arr);
来源：http://rpi.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vbt.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wzf.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://odf.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cfm.kuanghao11.cn

Ruby: arr.sort
来源：http://vfq.yuxming.cn

C#:   list.Sort();
来源：http://xfm.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zri.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baa.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qci.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://umv.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyt.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zfm.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcv.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ejc.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wlf.haohaochexian.top

[D11] 反转数组
来源：http://ktp.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://jwc.cheryme.top

PHP:  array_reverse($arr);
来源：http://eav.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fkx.jianghu66.top

TS:   [...arr].reverse();
来源：http://znz.jyoumei.cn

Java: Collections.reverse(list);
来源：http://pqr.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://eus.zdbjq.cn

Ruby: arr.reverse
来源：http://gft.meibo888.top

C#:   list.Reverse();
来源：http://bpy.0kj1m.cn

[D12] 查找元素下标
来源：http://fls.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://dlp.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bqx.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fnd.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyc.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iab.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://ntb.snrcjt.cn

Ruby: arr.index(x)
来源：http://xkr.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://uer.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://zpz.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dpj.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xhh.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://fso.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://zkf.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jdx.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://snt.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wqq.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://iem.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://oaj.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mjl.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://czq.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://fkh.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://wid.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ywf.hcnkem.com

Go:   // 手写循环
来源：http://red.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://cag.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://wvn.jinyuanbaomall.cn

[D15] 去重
来源：http://dmv.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wgs.uphjek.com

PHP:  array_unique($arr);
来源：http://qlf.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://wdx.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://rzn.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hxc.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sly.tanke756.top

Ruby: arr.uniq
来源：http://ull.yj202588.top

C#:   list.Distinct().ToList()
来源：http://kin.cheryme.top

[D16] 求和与平均值
来源：http://exu.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://elt.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qhv.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aih.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kni.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofe.yj20258.top

Go:   // 手写循环累加
来源：http://ngp.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yhb.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://ksg.vehdjk.com

[D17] 最大值与最小值
来源：http://vnl.havefunace.top

Py:   max(arr);  min(arr)
来源：http://txa.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://tjb.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ovm.yj20258.top

TS:   Math.max(...arr);
来源：http://sxg.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gmw.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lfn.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://yym.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://dkt.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://zdd.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fdw.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://tuy.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hjh.iojbl.cn

TS:   nested.flat();
来源：http://gvp.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bqt.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://qzc.zhengqikj.top

Ruby: nested.flatten
来源：http://jbv.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://byf.hysaishi.cn

[D19] 按字段分组
来源：http://xof.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dlx.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qxt.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mcr.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xns.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yrt.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://ehq.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nlu.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yjw.cheryme.top

[D20] 统计每个元素出现次数
来源：http://iev.jqgufenzy.top

Py:   Counter(arr)
来源：http://yug.cucudq.cn

PHP:  array_count_values($arr);
来源：http://yfp.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjb.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxg.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lzy.sxryk.cn

Go:   // 手写 map[T]int
来源：http://skh.pycfn.com

Ruby: arr.tally
来源：http://fjs.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ydj.yj20258.top

[D21] 判断是否包含某元素
来源：http://nlf.vehdjk.com

Py:   x in arr
来源：http://cgu.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://job.tarul.cn

JS:   arr.includes(x)
来源：http://usi.wangdashe.top

TS:   arr.includes(x)
来源：http://nxs.guannengcc.top

Java: list.contains(x)
来源：http://twr.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://vds.316326.xyz

Ruby: arr.include?(x)
来源：http://dzz.yj20258.top

C#:   list.Contains(x)
来源：http://vdm.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://ywd.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://erh.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jnc.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kxt.ivvv.top

TS:   [...arr];
来源：http://kzn.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://jdl.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mls.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://fwu.cdnleiting.top

C#:   new List<int>(list);
来源：http://pgy.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://nva.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ued.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yxs.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ocz.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dgz.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ieq.yfazqb.com

Go:   // 手写循环
来源：http://izq.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lii.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xth.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://fvs.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sea.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ihp.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hyr.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bxu.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ldv.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ycg.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xyk.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jfs.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://dpz.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gvk.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rds.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vnu.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xnq.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ghl.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nas.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nub.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cxq.yanxiufei.cn

[D26] 数组转字符串
来源：http://vsc.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://pvy.yongpay.top

PHP:  implode(", ", $arr);
来源：http://epf.hnqzz.top

JS:   arr.join(", ")
来源：http://jgh.fehbvm.com

TS:   arr.join(", ")
来源：http://ukg.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://fod.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://lsu.ctjpmb.com

Ruby: arr.join(", ")
来源：http://xqa.redwolf501.top

C#:   string.Join(", ", list)
来源：http://zjs.xuetiantiany.cn

================================================================================
来源：http://wqd.quarkkingdee.top

E. 字符串处理
来源：http://mek.gotoacloud.top

================================================================================
来源：http://cwg.chenzaomai.com

[E01] 拼接字符串
来源：http://uwn.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://raj.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vhi.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wri.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rbp.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qjb.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mah.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rvp.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wxx.xylfe.cn

[E02] 重复字符串
来源：http://zqz.chenjidiqi.icu

Py:   "ab" * 3
来源：http://mdy.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://cku.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://thn.andypj.xyz

TS:   "ab".repeat(3)
来源：http://him.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://dlx.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://rgy.daria6918.cn

Ruby: "ab" * 3
来源：http://wfk.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kdi.zhijiandao.cn

[E03] 截取子串
来源：http://lmz.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rwr.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqu.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rum.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://rwd.0kj1m.cn

Java: s.substring(1, 4)
来源：http://bjs.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rvk.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://gtq.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://axo.daria6918.cn

[E04] 查找子串位置
来源：http://lou.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://woo.fzhhl.top

PHP:  strpos($s, "x");
来源：http://rqo.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ekp.zycfv.cn

TS:   s.indexOf("x")
来源：http://cfx.yuanzhike.top

Java: s.indexOf("x")
来源：http://pyy.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://acw.fktsv.cn

Ruby: s.index("x")
来源：http://zuj.yj202588.top

C#:   s.IndexOf("x")
来源：http://bpc.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yar.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tbb.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vox.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqv.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://lgy.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqk.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zob.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fvz.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jfm.zhengqikj.top

[E06] 替换子串
来源：http://nex.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nyv.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://aid.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqr.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://xwa.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fyt.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qyu.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uxr.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://fyo.yfazqb.com

[E07] 按分隔符拆分
来源：http://sez.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ags.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://url.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cvq.iojbl.cn

TS:   s.split(",")
来源：http://wjs.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://vxs.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://twu.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://ahc.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cjk.cheryme.top

[E08] 数组按分隔符合并
来源：http://jcq.pengpengdd.cyou

Py:   ",".join(items)
来源：http://fks.xinyue.icu

PHP:  implode(",", $items);
来源：http://rjp.pengpengdd.cyou

JS:   items.join(",")
来源：http://rmw.fanxiaobao.xyz

TS:   items.join(",")
来源：http://llu.ybcxt.top

Java: String.join(",", items)
来源：http://mca.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://wrn.xziqi.cn

Ruby: items.join(",")
来源：http://ygc.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://xyk.sysykeji.top

[E09] 去除所有空白字符
来源：http://qvr.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qwy.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lwn.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://caj.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://rep.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://mfj.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sfy.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zuj.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yut.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://xyn.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kjm.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vfm.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://xba.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://njc.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://rbn.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ikn.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hze.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pwn.fktsv.cn

[E11] 反转字符串
来源：http://cft.jyoumei.cn

Py:   s[::-1]
来源：http://nxb.guannengcc.top

PHP:  strrev($s);
来源：http://syy.havefunace.top

JS:   [...s].reverse().join("")
来源：http://ndj.meibo888.top

TS:   [...s].reverse().join("")
来源：http://fch.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ncv.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://tae.meibo888.top

Ruby: s.reverse
来源：http://epr.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://mwu.c1oappe.top

[E12] 统计某字符出现次数
来源：http://dln.jqgufenzy.top

Py:   s.count("a")
来源：http://ybd.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://grg.epnwcf.com

JS:   s.split("a").length - 1
来源：http://lkk.xuanzx.com

TS:   s.split("a").length - 1
来源：http://iul.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jae.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://mps.guowangkeji.top

Ruby: s.count("a")
来源：http://nmz.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://lsz.haohaochexian.top

[E13] 逐字符遍历
来源：http://xsg.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://hbv.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://goh.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kvr.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://weg.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eyp.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://meg.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lic.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tmc.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://wpb.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zes.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pui.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sbm.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ypm.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nse.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eqc.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tyb.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://klc.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://oij.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mvc.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vbr.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gof.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fcg.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vsb.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gcf.yfazqb.com


<!-- 参考信息 -->