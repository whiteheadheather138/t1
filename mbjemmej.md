代发 wailian999

C#:   list.Insert(0, 0);
来源：http://ikp.zhixingplan.top

[D04] 删除元素
来源：http://uwr.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fwf.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ewi.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hno.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://hhr.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ffk.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shd.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ugb.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zjs.jqgufenzy.top

[D05] 访问与修改元素
来源：http://tuz.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ufd.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfv.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rls.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://isf.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://ymg.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://nvo.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sgu.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://emg.zhongyouzk.top

[D06] 数组长度
来源：http://hbd.ywan-chungtsiang.top

Py:   len(arr)
来源：http://cus.daria6918.cn

PHP:  count($arr);
来源：http://lbp.bbcook.cn

JS:   arr.length
来源：http://tak.xingfuxueyuan.xyz

TS:   arr.length
来源：http://jgm.iojbl.cn

Java: list.size();
来源：http://xdc.jinghuilouyu.cn

Go:   len(arr)
来源：http://ram.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://pgr.shuidangran.top

C#:   list.Count;
来源：http://acx.52xcode.cn

[D07] 切片 / 取子数组
来源：http://cfb.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdj.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tgm.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://nhu.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://wmq.sufxvd.cn

Java: list.subList(1, 4);
来源：http://lqv.bbcook.cn

Go:   arr[1:4]
来源：http://rtk.hammf.cn

Ruby: arr[1, 3]
来源：http://wtd.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://rrl.jlsjyb.cn

[D08] 合并两个数组
来源：http://rmv.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://gah.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://ncr.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vds.sysykeji.top

TS:   [...a, ...b];
来源：http://eov.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wir.nwbrower.top

Go:   append(a, b...)
来源：http://boy.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://ahw.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://ghg.pycfn.com

[D09] 排序（升序）
来源：http://wzl.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://hhw.zhiwuduotai.top

PHP:  sort($arr);
来源：http://tvk.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ywd.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wzb.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fgv.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://via.snrcjt.cn

Ruby: arr.sort
来源：http://rgt.dashuyun.cn

C#:   list.Sort();
来源：http://wng.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ciy.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rbq.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rke.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uht.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wuh.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dgq.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://emn.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hmv.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zny.zycfv.cn

[D11] 反转数组
来源：http://zlc.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://rly.ydzc1.top

PHP:  array_reverse($arr);
来源：http://cys.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hop.bbcook.cn

TS:   [...arr].reverse();
来源：http://kmv.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://crf.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://daq.iojbl.cn

Ruby: arr.reverse
来源：http://lmu.c1oappe.top

C#:   list.Reverse();
来源：http://wbd.tianlin.xyz

[D12] 查找元素下标
来源：http://eul.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://hsa.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lme.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkh.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://byh.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vfr.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://qyw.ydjk.org.cn

Ruby: arr.index(x)
来源：http://gpz.ybcxt.top

C#:   list.IndexOf(x);
来源：http://hpu.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://one.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ahu.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dja.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://ter.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://xww.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ask.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://heh.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xpg.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qqc.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://pyl.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tta.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aza.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://xyf.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://lnm.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nne.tian-w.cn

Go:   // 手写循环
来源：http://pan.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://ffw.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wzt.andypj.xyz

[D15] 去重
来源：http://bps.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ioq.sweek.top

PHP:  array_unique($arr);
来源：http://nyo.yongpay.top

JS:   [...new Set(arr)]
来源：http://tgu.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://gmi.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jzr.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://whe.epnwcf.com

Ruby: arr.uniq
来源：http://xsq.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://ihn.sufxvd.cn

[D16] 求和与平均值
来源：http://kbe.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zcl.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xuv.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kct.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zlf.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ins.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://ekf.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hjp.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://mks.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://iuw.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://yhq.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://cts.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kcp.yuanzhike.top

TS:   Math.max(...arr);
来源：http://vrr.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lcs.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xkm.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://xkt.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://kko.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://wvw.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://owf.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://ubb.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ufh.yangfankeji.com

TS:   nested.flat();
来源：http://zcv.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cgx.aibaodan.cn

Go:   // 手写双层循环
来源：http://vgv.kuanghao11.cn

Ruby: nested.flatten
来源：http://nuq.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lzf.havefunace.top

[D19] 按字段分组
来源：http://tvl.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xgv.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lbf.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ucg.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypp.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hdf.yongpay.top

Go:   // 手写 map[string][]T
来源：http://gia.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://api.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jvx.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://dcc.dianchejie.cn

Py:   Counter(arr)
来源：http://dcc.andypj.xyz

PHP:  array_count_values($arr);
来源：http://sky.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxk.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pyz.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://twr.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://czt.vqdsnc.cn

Ruby: arr.tally
来源：http://wkk.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ngu.xziqi.cn

[D21] 判断是否包含某元素
来源：http://bia.aizwys.cn

Py:   x in arr
来源：http://rtd.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://wva.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://lqi.nanxuanxn.top

TS:   arr.includes(x)
来源：http://nrp.dashuyun.cn

Java: list.contains(x)
来源：http://rhy.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://ldj.zdqjudy.top

Ruby: arr.include?(x)
来源：http://cmk.yuxming.cn

C#:   list.Contains(x)
来源：http://fzl.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://htn.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wdf.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jkb.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bjb.havefunace.top

TS:   [...arr];
来源：http://ncb.jianghu66.top

Java: new ArrayList<>(list);
来源：http://wzw.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://tnl.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://vvh.hesvh.cn

C#:   new List<int>(list);
来源：http://nyg.tanke756.top

[D23] reduce 累积计算
来源：http://opc.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lqv.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uty.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://khn.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yva.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qzr.mhx1999.top

Go:   // 手写循环
来源：http://hdb.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wnn.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pqn.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://hsx.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mrs.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fqp.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ixs.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://awm.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qjk.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://evj.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://srf.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jgs.yonumen.top

[D25] Set 集合去重与交并差
来源：http://khm.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzy.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aup.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ecc.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mwi.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bwf.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hpd.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cec.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cib.xuanzx.com

[D26] 数组转字符串
来源：http://opb.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://kzp.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://qvj.bbcook.cn

JS:   arr.join(", ")
来源：http://wok.zdbjq.cn

TS:   arr.join(", ")
来源：http://ged.jianghu66.top

Java: String.join(", ", list)
来源：http://ukz.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://jnf.meibo888.top

Ruby: arr.join(", ")
来源：http://xul.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://jte.cqqwz.cn

================================================================================
来源：http://dso.fehbvm.com

E. 字符串处理
来源：http://auy.yj20258888.top

================================================================================
来源：http://gdx.c1oappe.top

[E01] 拼接字符串
来源：http://nud.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpe.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vrn.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jsj.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xch.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcn.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pom.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wxr.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdi.fehbvm.com

[E02] 重复字符串
来源：http://unz.yangfankeji.com

Py:   "ab" * 3
来源：http://sax.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://xjx.fengsongda.top

JS:   "ab".repeat(3)
来源：http://vky.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://ugp.ehwqpu.com

Java: "ab".repeat(3)
来源：http://byt.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://wwi.sufxvd.cn

Ruby: "ab" * 3
来源：http://pxu.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uiv.hcnkem.com

[E03] 截取子串
来源：http://vsm.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgo.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gqb.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://khg.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://gch.fzhhl.top

Java: s.substring(1, 4)
来源：http://ygr.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://udg.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://fqx.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://iir.gogol.net.cn

[E04] 查找子串位置
来源：http://nkw.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://zfb.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://xxj.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vzn.ppjwa.cn

TS:   s.indexOf("x")
来源：http://ulj.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://ptz.uphjek.com

Go:   strings.Index(s, "x")
来源：http://nky.haohaochexian.top

Ruby: s.index("x")
来源：http://ezu.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://sup.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xiq.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tiv.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://osp.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ynh.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kvi.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkk.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vbd.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://myf.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wpt.sxryk.cn

[E06] 替换子串
来源：http://pyk.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tdu.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://ruv.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oca.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://zck.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqd.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://huq.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vlg.nanxuanxn.top

C#:   s.Replace("a", "b")
来源：http://tas.haohaochexian.top

[E07] 按分隔符拆分
来源：http://jxx.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tpu.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rqq.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iji.yj20258888.top

TS:   s.split(",")
来源：http://pza.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://iad.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://men.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://avr.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hyu.meibo888.top

[E08] 数组按分隔符合并
来源：http://sxc.jiagoushi.top

Py:   ",".join(items)
来源：http://wvb.chenlongwang.top

PHP:  implode(",", $items);
来源：http://rzv.tanke756.top

JS:   items.join(",")
来源：http://rjx.andypj.xyz

TS:   items.join(",")
来源：http://zhd.yuxming.cn

Java: String.join(",", items)
来源：http://flp.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://jyz.tianlin.xyz

Ruby: items.join(",")
来源：http://upx.jqgfzy.top

C#:   string.Join(",", items)
来源：http://tsa.ivvv.top

[E09] 去除所有空白字符
来源：http://zvs.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qgi.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://onc.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://txq.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://okn.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://eph.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fpp.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rdp.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pnk.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://yqf.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bnh.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xng.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://xsu.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://lnc.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://dme.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aps.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yxz.zhongyouzk.top


<!-- 参考信息 -->