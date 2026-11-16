代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gxn.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pzd.ppjwa.cn

[D05] 访问与修改元素
来源：http://amd.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kqm.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://snj.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hlr.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://cng.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://nqs.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://gsk.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aha.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ayn.jinyuanbaomall.cn

[D06] 数组长度
来源：http://raj.bjfxy.top

Py:   len(arr)
来源：http://giy.fktsv.cn

PHP:  count($arr);
来源：http://gxy.zhoulong.xyz

JS:   arr.length
来源：http://bhn.xingfuxueyuan.xyz

TS:   arr.length
来源：http://xdr.yonumen.top

Java: list.size();
来源：http://jrt.pycfn.com

Go:   len(arr)
来源：http://gtp.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://wox.dashuyun.cn

C#:   list.Count;
来源：http://eha.tanke756.top

[D07] 切片 / 取子数组
来源：http://jnd.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ctv.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nuh.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://rbo.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://tim.meibo888.top

Java: list.subList(1, 4);
来源：http://qwt.gaohongyu789.top

Go:   arr[1:4]
来源：http://pip.ydzc1.top

Ruby: arr[1, 3]
来源：http://yfn.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://edf.hnqzz.top

[D08] 合并两个数组
来源：http://gdn.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://oyi.uphjek.com

PHP:  array_merge($a, $b);
来源：http://bnm.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lkv.meibo888.top

TS:   [...a, ...b];
来源：http://dpw.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fhi.ydzc1.top

Go:   append(a, b...)
来源：http://huy.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://jfg.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://iiy.c1oappe.top

[D09] 排序（升序）
来源：http://wio.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://wyx.guowangkeji.top

PHP:  sort($arr);
来源：http://gbc.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fqw.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lmh.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mui.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vfj.sweek.top

Ruby: arr.sort
来源：http://nqf.fanxiaobao.xyz

C#:   list.Sort();
来源：http://ipo.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://sby.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tqx.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhp.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gtc.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aot.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ifh.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kew.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xld.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xpb.tianlin.xyz

[D11] 反转数组
来源：http://xsg.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://apn.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://tgv.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ozk.yj20258.top

TS:   [...arr].reverse();
来源：http://xxf.fzhhl.top

Java: Collections.reverse(list);
来源：http://scy.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://zji.hongshengwenyu.top

Ruby: arr.reverse
来源：http://ihy.vqdsnc.cn

C#:   list.Reverse();
来源：http://qoy.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://plr.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://swd.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ebl.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wee.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjm.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pbb.yj202588.top

Go:   slices.Index(arr, x)
来源：http://wzx.chenlongwang.top

Ruby: arr.index(x)
来源：http://qax.yj202588.top

C#:   list.IndexOf(x);
来源：http://vno.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://vhs.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xat.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gpx.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://tqw.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://ffi.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zvp.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odr.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://ncx.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://aht.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://tht.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://taq.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dfi.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://hjo.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://nuo.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lzu.shzxlz.cn

Go:   // 手写循环
来源：http://qaz.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gbz.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qid.xingfuxueyuan.xyz

[D15] 去重
来源：http://kag.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eyy.yvedp.cn

PHP:  array_unique($arr);
来源：http://mzn.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://xry.zycfv.cn

TS:   [...new Set(arr)]
来源：http://ttp.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mwv.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rnr.xinyue.icu

Ruby: arr.uniq
来源：http://qyj.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://syz.cheryme.top

[D16] 求和与平均值
来源：http://bhl.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hev.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://taw.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iky.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aij.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cwx.c1oappe.top

Go:   // 手写循环累加
来源：http://tor.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pti.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://dbo.jianghu66.top

[D17] 最大值与最小值
来源：http://hgw.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://yar.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://sgm.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uxa.daria6918.cn

TS:   Math.max(...arr);
来源：http://hrr.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cdk.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://guv.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://tjo.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://ueh.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://lxy.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rhn.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://wla.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rzg.meibo888.top

TS:   nested.flat();
来源：http://qox.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://efm.meibo888.top

Go:   // 手写双层循环
来源：http://iju.gaohongyu789.top

Ruby: nested.flatten
来源：http://rmg.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhg.316326.xyz

[D19] 按字段分组
来源：http://mzz.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hrm.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bmd.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zzv.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ulh.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://adw.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://kud.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lbr.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eod.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://tin.guowangkeji.top

Py:   Counter(arr)
来源：http://mzw.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://qbd.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxw.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://frg.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ves.xylfe.cn

Go:   // 手写 map[T]int
来源：http://txk.feifeiyinyue.top

Ruby: arr.tally
来源：http://vxc.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tky.cashguo.top

[D21] 判断是否包含某元素
来源：http://adq.jqgfzy.top

Py:   x in arr
来源：http://rgn.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://oiz.fktsv.cn

JS:   arr.includes(x)
来源：http://rgi.vehdjk.com

TS:   arr.includes(x)
来源：http://vfq.redwolf501.top

Java: list.contains(x)
来源：http://rwa.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://buu.zycfv.cn

Ruby: arr.include?(x)
来源：http://fpg.zdqjudy.top

C#:   list.Contains(x)
来源：http://abf.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://nkn.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kko.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rea.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ymu.hywenlv.cn

TS:   [...arr];
来源：http://vqm.hesvh.cn

Java: new ArrayList<>(list);
来源：http://ixf.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://zcn.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://okj.aizwys.cn

C#:   new List<int>(list);
来源：http://xec.c1oappe.top

[D23] reduce 累积计算
来源：http://xpo.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zoi.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lur.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqi.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xxe.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cbj.yongpay.top

Go:   // 手写循环
来源：http://yxz.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jvj.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aui.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://otj.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zub.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cyc.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vgr.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uag.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fsq.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ivf.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dtl.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xta.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://uqq.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ljo.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uyr.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://otn.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vup.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ppv.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://adj.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jah.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gbs.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://nnj.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://gqx.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://unq.yj20258888.top

JS:   arr.join(", ")
来源：http://wtn.hfpthk.cn

TS:   arr.join(", ")
来源：http://woe.yuanzhike.top

Java: String.join(", ", list)
来源：http://etn.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://fit.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://xol.xinyue.icu

C#:   string.Join(", ", list)
来源：http://duv.aizwys.cn

================================================================================
来源：http://luv.xinyue.icu

E. 字符串处理
来源：http://gzc.zdbjq.cn

================================================================================
来源：http://xxl.nanxuanxn.top

[E01] 拼接字符串
来源：http://goj.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fxr.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iat.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbc.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hmd.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rxz.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gav.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lgc.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pbn.9152youxi.cn

[E02] 重复字符串
来源：http://ndg.zhongyouzk.top

Py:   "ab" * 3
来源：http://rfc.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://hko.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://evt.fehbvm.com

TS:   "ab".repeat(3)
来源：http://chg.hammf.cn

Java: "ab".repeat(3)
来源：http://lxg.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://vtm.chenlongwang.top

Ruby: "ab" * 3
来源：http://yjv.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mse.quarkkingdee.top

[E03] 截取子串
来源：http://lhx.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jxu.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rcn.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvf.yfazqb.com

TS:   s.slice(1, 4)
来源：http://uar.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://mla.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kow.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://vba.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://iul.zhixingplan.top

[E04] 查找子串位置
来源：http://azl.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://bvm.cashguo.top

PHP:  strpos($s, "x");
来源：http://ylo.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rom.zdbjq.cn

TS:   s.indexOf("x")
来源：http://mev.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://mqu.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://pue.dashuyun.cn

Ruby: s.index("x")
来源：http://fep.epnwcf.com

C#:   s.IndexOf("x")
来源：http://mke.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://lij.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txb.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jsf.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpo.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jhj.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qsc.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gzi.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://axc.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://prx.redwolf501.top

[E06] 替换子串
来源：http://vab.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xti.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://mws.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujg.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://yuh.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tvn.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jaw.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dkh.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://wfk.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://bat.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://urs.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mho.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cdv.quarkkingdee.top

TS:   s.split(",")
来源：http://sla.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://lru.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xze.tarul.cn

Ruby: s.split(",");  s.split
来源：http://myr.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ktq.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://wfn.yj202588.top

Py:   ",".join(items)
来源：http://zdg.cqqwz.cn

PHP:  implode(",", $items);
来源：http://mwf.fengsongda.top

JS:   items.join(",")
来源：http://xys.zdqjudy.top

TS:   items.join(",")
来源：http://xtx.pengpengdd.cyou

Java: String.join(",", items)
来源：http://hhu.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://juq.guowangkeji.top

Ruby: items.join(",")
来源：http://vxr.52xcode.cn

C#:   string.Join(",", items)
来源：http://hwp.zhengqikj.top

[E09] 去除所有空白字符
来源：http://lzj.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bok.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cpk.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://bjo.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://ejr.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://iom.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://obk.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qon.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xqx.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://dzv.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bpe.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pqj.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://geb.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://wcz.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://qhp.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hya.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qrt.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fcn.sweek.top

[E11] 反转字符串
来源：http://zvg.yfazqb.com

Py:   s[::-1]
来源：http://idd.aizwys.cn

PHP:  strrev($s);
来源：http://yak.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://ujh.yj20258.top

TS:   [...s].reverse().join("")
来源：http://jro.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hme.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ttv.52xcode.cn


<!-- 参考信息 -->