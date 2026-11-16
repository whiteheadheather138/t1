代发 wailian999

PHP:  sort($arr);
来源：http://aaq.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://epp.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://epo.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jjw.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://thi.sweek.top

Ruby: arr.sort
来源：http://itd.yonumen.top

C#:   list.Sort();
来源：http://dbx.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zml.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mtx.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yha.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylo.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bfk.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ilt.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ldd.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sqo.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qbw.quarkkingdee.top

[D11] 反转数组
来源：http://xsm.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://fpi.wangdashe.top

PHP:  array_reverse($arr);
来源：http://rot.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vlp.ydzc1.top

TS:   [...arr].reverse();
来源：http://vta.ydzc1.top

Java: Collections.reverse(list);
来源：http://ool.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://jsn.tianlin.xyz

Ruby: arr.reverse
来源：http://ytz.yuanzhike.top

C#:   list.Reverse();
来源：http://mrb.vehdjk.com

[D12] 查找元素下标
来源：http://oew.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://lzu.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qoc.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vix.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzp.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://egq.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://bzn.ppjwa.cn

Ruby: arr.index(x)
来源：http://bru.52xcode.cn

C#:   list.IndexOf(x);
来源：http://hvo.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://yqv.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gui.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zti.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://jjl.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://qdw.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bzn.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uit.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://jsc.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ynv.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://xbi.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ccx.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wco.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://myv.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://mir.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvo.chenlongwang.top

Go:   // 手写循环
来源：http://qhg.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://lyn.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://odf.andypj.xyz

[D15] 去重
来源：http://civ.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qgl.hesvh.cn

PHP:  array_unique($arr);
来源：http://kus.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://bbh.ivvv.top

TS:   [...new Set(arr)]
来源：http://byw.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pjr.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://bnn.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://qpc.uphjek.com

C#:   list.Distinct().ToList()
来源：http://wnm.ctjpmb.com

[D16] 求和与平均值
来源：http://jvl.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xbi.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hrk.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnn.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wtc.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sxb.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://cia.zhongyouzk.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvh.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://tkd.ybcxt.top

[D17] 最大值与最小值
来源：http://efv.ivvv.top

Py:   max(arr);  min(arr)
来源：http://wsk.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://wui.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yif.smart0.xyz

TS:   Math.max(...arr);
来源：http://rml.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://idc.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tzf.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://ffu.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://pnx.tarul.cn

[D18] 扁平化嵌套数组
来源：http://jdg.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jbq.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://wya.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wsv.xuanzx.com

TS:   nested.flat();
来源：http://rnw.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vwq.zdqjudy.top

Go:   // 手写双层循环
来源：http://wan.gogol.net.cn

Ruby: nested.flatten
来源：http://mwo.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yhv.shzxlz.cn

[D19] 按字段分组
来源：http://ltr.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://guu.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kvr.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rci.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xtz.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xxv.sweek.top

Go:   // 手写 map[string][]T
来源：http://axv.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ylg.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vmm.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://jbo.dashuyun.cn

Py:   Counter(arr)
来源：http://tsg.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://bfr.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://szv.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyk.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ujs.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://wvp.c1oappe.top

Ruby: arr.tally
来源：http://mgq.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kwp.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://lys.epnwcf.com

Py:   x in arr
来源：http://hqv.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://vnr.chenlongwang.top

JS:   arr.includes(x)
来源：http://ygl.yuanzhike.top

TS:   arr.includes(x)
来源：http://uax.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://wqe.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://elr.gotoacloud.top

Ruby: arr.include?(x)
来源：http://ozo.yfazqb.com

C#:   list.Contains(x)
来源：http://hjz.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://tlb.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gzv.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aee.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tvr.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://biv.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://ybs.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://mus.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://pkq.tian-w.cn

C#:   new List<int>(list);
来源：http://wly.nwbrower.top

[D23] reduce 累积计算
来源：http://asa.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yhd.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xok.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyu.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rxq.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ned.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://mrb.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fmz.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xkl.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://srq.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://piy.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sqo.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://drm.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://urc.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://glf.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bhx.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lmo.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vin.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://ckx.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wdf.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hmf.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bih.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://prv.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dkq.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oyl.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xpa.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qju.sysykeji.top

[D26] 数组转字符串
来源：http://poy.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://wmo.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://wcl.bbcook.cn

JS:   arr.join(", ")
来源：http://lnn.zdqjudy.top

TS:   arr.join(", ")
来源：http://pun.jinqigufen.top

Java: String.join(", ", list)
来源：http://hyg.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://axe.cdnleiting.top

Ruby: arr.join(", ")
来源：http://lhk.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://ked.vehdjk.com

================================================================================
来源：http://wei.cdnleiting.top

E. 字符串处理
来源：http://qqc.jianghu66.top

================================================================================
来源：http://jyj.jinqigfzy.top

[E01] 拼接字符串
来源：http://zdn.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dqh.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dhk.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxv.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jhx.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fod.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qtx.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iyz.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lwl.cheryme.top

[E02] 重复字符串
来源：http://ynl.sjlbkw.cn

Py:   "ab" * 3
来源：http://ouf.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://zhg.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://rtr.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://vkv.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://khq.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://rkm.xuanzx.com

Ruby: "ab" * 3
来源：http://bnh.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oyy.aizwys.cn

[E03] 截取子串
来源：http://clk.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xan.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bvp.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lad.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://jpg.iojbl.cn

Java: s.substring(1, 4)
来源：http://fem.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fos.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ici.ivvv.top

C#:   s.Substring(1, 3)
来源：http://nxq.cashguo.top

[E04] 查找子串位置
来源：http://rks.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://hqo.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://cfx.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yeh.hysaishi.cn

TS:   s.indexOf("x")
来源：http://aft.cheryme.top

Java: s.indexOf("x")
来源：http://yfw.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://vub.xuetiantiany.cn

Ruby: s.index("x")
来源：http://gid.havefunace.top

C#:   s.IndexOf("x")
来源：http://kme.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlp.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://elj.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tkj.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glb.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bju.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tnj.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fdw.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cmu.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dfa.vehdjk.com

[E06] 替换子串
来源：http://pfv.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dlz.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://axw.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxp.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://gpf.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xrx.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://box.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ozi.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://ncy.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://dra.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wkg.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hoc.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://jms.daria6918.cn

TS:   s.split(",")
来源：http://uzv.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://wjp.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wlz.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://kzg.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fmq.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://imq.sysykeji.top

Py:   ",".join(items)
来源：http://voo.hcnkem.com

PHP:  implode(",", $items);
来源：http://vhp.ybcxt.top

JS:   items.join(",")
来源：http://pso.yueranfly.top

TS:   items.join(",")
来源：http://xdo.havefunace.top

Java: String.join(",", items)
来源：http://pjq.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://hsw.mhx1999.top

Ruby: items.join(",")
来源：http://csq.ivvv.top

C#:   string.Join(",", items)
来源：http://eyt.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://wmv.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ien.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://msq.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://wxs.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://mkg.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://lhc.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://auk.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ixt.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvb.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://udt.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dsh.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fbl.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://mob.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://iiw.zycfv.cn

Java: String.format("%03d", 7)
来源：http://ytt.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lpe.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ljf.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uiu.epnwcf.com

[E11] 反转字符串
来源：http://odi.dashuyun.cn

Py:   s[::-1]
来源：http://eqf.tarul.cn

PHP:  strrev($s);
来源：http://xac.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://kud.yj20258.top

TS:   [...s].reverse().join("")
来源：http://gas.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ogv.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://omv.shuidangran.top

Ruby: s.reverse
来源：http://asp.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zoj.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://xyw.316326.xyz

Py:   s.count("a")
来源：http://ecm.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://jbh.andypj.xyz

JS:   s.split("a").length - 1
来源：http://odu.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://cdp.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://plv.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://kau.sweek.top

Ruby: s.count("a")
来源：http://kjg.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://lgz.shuidangran.top

[E13] 逐字符遍历
来源：http://qhq.pycfn.com

Py:   for ch in s: print(ch)
来源：http://shc.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mjh.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cup.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ezp.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://saq.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hjt.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kjk.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xaf.fktsv.cn

[E14] URL 编码与 Base64
来源：http://syq.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://etw.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://stf.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ycv.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zul.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xso.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ztt.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyj.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oaa.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://zpe.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xjl.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hse.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tyj.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://gne.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://enc.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ipq.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eso.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qsn.andypj.xyz

[E16] 数字千分位
来源：http://low.sxryk.cn

Py:   f"{1234567:,}"
来源：http://qhl.jqgfzy.top


<!-- 参考信息 -->