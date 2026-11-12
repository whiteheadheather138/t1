代发 wailian999

C#:   list.Insert(0, 0);
来源：http://uhi.shanyushiyangkeji.top

[D04] 删除元素
来源：http://fzx.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://akl.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hqd.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vpf.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://htv.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tiy.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tft.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mid.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xyq.ydzc1.top

[D05] 访问与修改元素
来源：http://cio.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rys.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yzy.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yrp.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://jkt.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://oqx.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://mea.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pfh.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rzw.andypj.xyz

[D06] 数组长度
来源：http://eik.hammf.cn

Py:   len(arr)
来源：http://lat.svipenyu.cn

PHP:  count($arr);
来源：http://tin.jyoumei.cn

JS:   arr.length
来源：http://xop.fehbvm.com

TS:   arr.length
来源：http://fyh.zhiwuduotai.top

Java: list.size();
来源：http://smu.xylfe.cn

Go:   len(arr)
来源：http://wai.bjfxy.top

Ruby: arr.length; arr.size
来源：http://ydr.jqgufenzy.top

C#:   list.Count;
来源：http://nhy.sxryk.cn

[D07] 切片 / 取子数组
来源：http://ffj.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ymv.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qtl.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://sdd.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://bxz.xylfe.cn

Java: list.subList(1, 4);
来源：http://pvj.zhongyouzk.top

Go:   arr[1:4]
来源：http://xal.shzxlz.cn

Ruby: arr[1, 3]
来源：http://rua.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://kju.sxryk.cn

[D08] 合并两个数组
来源：http://aws.jlsjyb.cn

Py:   a + b;  a.extend(b)
来源：http://rpl.yonumen.top

PHP:  array_merge($a, $b);
来源：http://maw.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pqa.yonumen.top

TS:   [...a, ...b];
来源：http://ddv.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ihi.havefunace.top

Go:   append(a, b...)
来源：http://lbj.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://kza.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://rhz.jianghu66.top

[D09] 排序（升序）
来源：http://beh.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://bmo.jlsjyb.cn

PHP:  sort($arr);
来源：http://cvr.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pnm.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ide.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rjv.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://swu.zdbjq.cn

Ruby: arr.sort
来源：http://afw.bbcook.cn

C#:   list.Sort();
来源：http://gjb.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vdu.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xes.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://djf.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ihq.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qtd.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rlp.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tyt.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vwn.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kfq.jyoumei.cn

[D11] 反转数组
来源：http://eqh.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qzo.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://utj.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bzg.yuxming.cn

TS:   [...arr].reverse();
来源：http://upe.gotoacloud.top

Java: Collections.reverse(list);
来源：http://ztn.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://bxh.hysaishi.cn

Ruby: arr.reverse
来源：http://hah.nanxuanxn.top

C#:   list.Reverse();
来源：http://nkx.xuetiantiany.cn

[D12] 查找元素下标
来源：http://wok.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://dbc.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zkg.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iow.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vnm.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gjl.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://wyx.epnwcf.com

Ruby: arr.index(x)
来源：http://dkn.xylfe.cn

C#:   list.IndexOf(x);
来源：http://yfa.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://mfa.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qaj.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xhc.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://mla.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://ape.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fhg.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rjy.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ykb.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://nht.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://jsw.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jqf.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gem.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://jqw.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://gue.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kjb.wangdashe.top

Go:   // 手写循环
来源：http://lex.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://ijf.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eho.jinqigfzy.top

[D15] 去重
来源：http://imb.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xuf.ctjpmb.com

PHP:  array_unique($arr);
来源：http://bdm.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://gdf.andypj.xyz

TS:   [...new Set(arr)]
来源：http://kwr.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ntj.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mpp.fehbvm.com

Ruby: arr.uniq
来源：http://cxm.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://abq.redwolf501.top

[D16] 求和与平均值
来源：http://bhl.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://asl.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mqb.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajr.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jnc.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tdq.yvedp.cn

Go:   // 手写循环累加
来源：http://lxi.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ijn.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://gwp.jyoumei.cn

[D17] 最大值与最小值
来源：http://mcv.tanke756.top

Py:   max(arr);  min(arr)
来源：http://ogb.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://wgz.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jbg.xziqi.cn

TS:   Math.max(...arr);
来源：http://kxp.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kjt.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ojd.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://efv.sweek.top

C#:   list.Max();  list.Min()
来源：http://mhc.cashguo.top

[D18] 扁平化嵌套数组
来源：http://eoy.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nrr.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://uxo.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://plm.ppjwa.cn

TS:   nested.flat();
来源：http://jwn.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yaf.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://dxa.chenzaomai.com

Ruby: nested.flatten
来源：http://teu.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ewa.tarul.cn

[D19] 按字段分组
来源：http://zzq.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zpx.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qsd.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vxf.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://soj.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://olm.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://qny.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pie.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qdn.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://aul.shangyingyoupin.top

Py:   Counter(arr)
来源：http://plc.fzhhl.top

PHP:  array_count_values($arr);
来源：http://vuo.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sni.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvy.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zfc.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://ngl.gzhubu.top

Ruby: arr.tally
来源：http://fqm.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jll.aizwys.cn

[D21] 判断是否包含某元素
来源：http://han.jiagoushi.top

Py:   x in arr
来源：http://egf.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://qfq.gogol.net.cn

JS:   arr.includes(x)
来源：http://txs.chenzaomai.com

TS:   arr.includes(x)
来源：http://iab.zycfv.cn

Java: list.contains(x)
来源：http://eiw.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://yhv.yonumen.top

Ruby: arr.include?(x)
来源：http://lyp.xuanzx.com

C#:   list.Contains(x)
来源：http://qpm.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://nbe.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oey.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fky.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://evr.smart0.xyz

TS:   [...arr];
来源：http://fwo.tarul.cn

Java: new ArrayList<>(list);
来源：http://rit.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lmm.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://pvb.gzhubu.top

C#:   new List<int>(list);
来源：http://lgt.hysaishi.cn

[D23] reduce 累积计算
来源：http://kex.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vgg.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://khs.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmr.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnl.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://srs.yonumen.top

Go:   // 手写循环
来源：http://lmd.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfu.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mfw.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://imd.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nom.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dyh.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kvh.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tcq.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yqv.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dll.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://igg.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://slb.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://gzz.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fwu.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ilf.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eet.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://acg.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ndy.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zvo.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://diu.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mhs.bbcook.cn

[D26] 数组转字符串
来源：http://uio.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://yue.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://vsf.bbcook.cn

JS:   arr.join(", ")
来源：http://cbv.aizwys.cn

TS:   arr.join(", ")
来源：http://doz.snrcjt.cn

Java: String.join(", ", list)
来源：http://dnj.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://hqo.aizwys.cn

Ruby: arr.join(", ")
来源：http://yrh.sxryk.cn

C#:   string.Join(", ", list)
来源：http://lhp.wangshuangyany.cn

================================================================================
来源：http://vvd.hesvh.cn

E. 字符串处理
来源：http://gdw.vehdjk.com

================================================================================
来源：http://ode.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://upf.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gpf.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bng.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpi.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rlh.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vbp.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qhe.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yov.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tie.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://ggc.zdqjudy.top

Py:   "ab" * 3
来源：http://udq.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://cbp.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://brm.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://zee.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://xjb.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://qdl.jinqigufen.top

Ruby: "ab" * 3
来源：http://oye.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://otd.zdqjudy.top

[E03] 截取子串
来源：http://xfo.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://roh.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jfw.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bva.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://ekt.yueranfly.top

Java: s.substring(1, 4)
来源：http://trf.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rdv.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://zme.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://ikn.dianchejie.cn

[E04] 查找子串位置
来源：http://zuk.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://hea.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://jtj.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xrv.hammf.cn

TS:   s.indexOf("x")
来源：http://prb.nwbrower.top

Java: s.indexOf("x")
来源：http://itt.pycfn.com

Go:   strings.Index(s, "x")
来源：http://pbm.tian-w.cn

Ruby: s.index("x")
来源：http://udh.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://scy.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://whf.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dod.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mhg.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kdy.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pjs.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhp.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://szw.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bhg.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uya.cdnleiting.top

[E06] 替换子串
来源：http://yvx.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zhl.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://hus.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbp.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://epp.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwc.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gjf.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://phq.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://vje.mhx1999.top

[E07] 按分隔符拆分
来源：http://qsa.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qjo.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqh.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dbd.aizwys.cn

TS:   s.split(",")
来源：http://igc.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tfz.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nhn.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://yzs.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ubr.xinyue.icu

[E08] 数组按分隔符合并
来源：http://ilf.sufxvd.cn

Py:   ",".join(items)
来源：http://nxn.sufxvd.cn

PHP:  implode(",", $items);
来源：http://nvh.haohaochexian.top

JS:   items.join(",")
来源：http://mhv.zhiwuduotai.top

TS:   items.join(",")
来源：http://uue.shzxlz.cn

Java: String.join(",", items)
来源：http://uqe.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://fmm.snrcjt.cn

Ruby: items.join(",")
来源：http://zcs.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://vcd.yueranfly.top

[E09] 去除所有空白字符
来源：http://lhp.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ijd.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ksj.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://lxg.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://meu.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://luy.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://gbs.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://fmn.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gwg.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://yrn.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jev.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pgd.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://xlt.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://wcj.bjfxy.top

Java: String.format("%03d", 7)
来源：http://twh.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ixh.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkp.jinghuilouyu.cn


<!-- 参考信息 -->