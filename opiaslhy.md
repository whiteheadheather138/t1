代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gah.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cza.zycfv.cn

[D05] 访问与修改元素
来源：http://fjk.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xhi.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cke.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ixz.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://mxs.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://gxw.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://wzq.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bet.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eaa.jinqigfzy.top

[D06] 数组长度
来源：http://dvp.cashguo.top

Py:   len(arr)
来源：http://jlp.nwbrower.top

PHP:  count($arr);
来源：http://mme.zhengqikj.top

JS:   arr.length
来源：http://nzi.dianchejie.cn

TS:   arr.length
来源：http://liv.xuetiantiany.cn

Java: list.size();
来源：http://upl.hcnkem.com

Go:   len(arr)
来源：http://wvv.yfazqb.com

Ruby: arr.length; arr.size
来源：http://pir.gzhubu.top

C#:   list.Count;
来源：http://udr.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://wtl.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jth.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cca.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://osb.cheryme.top

TS:   arr.slice(1, 4);
来源：http://sdm.yj202588.top

Java: list.subList(1, 4);
来源：http://fcc.yonumen.top

Go:   arr[1:4]
来源：http://wvt.smart0.xyz

Ruby: arr[1, 3]
来源：http://wle.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://mdr.yongpay.top

[D08] 合并两个数组
来源：http://iof.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://cms.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://aur.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://joy.jyoumei.cn

TS:   [...a, ...b];
来源：http://hbt.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xmr.jqgfzy.top

Go:   append(a, b...)
来源：http://qde.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://mew.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://jln.redwolf501.top

[D09] 排序（升序）
来源：http://cjm.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://gfn.tian-w.cn

PHP:  sort($arr);
来源：http://dly.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zhe.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kvr.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rzx.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pkv.guowangkeji.top

Ruby: arr.sort
来源：http://qps.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://fva.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://iku.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vds.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cck.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://und.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ilv.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xpo.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rlq.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zeq.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ooi.smart0.xyz

[D11] 反转数组
来源：http://qik.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://toi.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://uzf.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://doo.xziqi.cn

TS:   [...arr].reverse();
来源：http://ydl.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://dkd.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://nyb.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://jtl.svipenyu.cn

C#:   list.Reverse();
来源：http://zkl.zhijiandao.cn

[D12] 查找元素下标
来源：http://zlj.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://fbn.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://svb.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://unk.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qqf.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vuw.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://djb.hesvh.cn

Ruby: arr.index(x)
来源：http://ywn.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://afw.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://cdo.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jiy.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tsd.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://cqm.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://qyc.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cvs.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kwt.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://rsr.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cjm.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://rqr.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://scl.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xxf.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://hou.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://kjt.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://coa.cashguo.top

Go:   // 手写循环
来源：http://len.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vms.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nxa.jinyuanbaomall.cn

[D15] 去重
来源：http://paj.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fpo.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://hgd.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://pqm.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://pwt.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dpm.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uqk.vehdjk.com

Ruby: arr.uniq
来源：http://pwr.yonumen.top

C#:   list.Distinct().ToList()
来源：http://lor.zdqjudy.top

[D16] 求和与平均值
来源：http://mqj.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zgy.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bio.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wwb.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://del.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xzm.meibo888.top

Go:   // 手写循环累加
来源：http://blx.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nsg.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://dci.9152youxi.cn

[D17] 最大值与最小值
来源：http://zvi.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://pzf.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://ndp.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lkz.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://qcz.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ipq.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kvq.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://qcq.tanke756.top

C#:   list.Max();  list.Min()
来源：http://zuc.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://jkn.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yuh.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://mew.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mml.snrcjt.cn

TS:   nested.flat();
来源：http://vff.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://srd.cucudq.cn

Go:   // 手写双层循环
来源：http://iyk.c1oappe.top

Ruby: nested.flatten
来源：http://fut.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wog.fehbvm.com

[D19] 按字段分组
来源：http://qqi.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oro.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vel.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://urq.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fcj.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zge.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://vje.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://las.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bvs.tarul.cn

[D20] 统计每个元素出现次数
来源：http://bir.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://fbu.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://sjq.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tly.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jzg.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ugu.birdmap.top

Go:   // 手写 map[T]int
来源：http://rcj.dashuyun.cn

Ruby: arr.tally
来源：http://mmz.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wga.tanke756.top

[D21] 判断是否包含某元素
来源：http://nqi.xingfuxueyuan.xyz

Py:   x in arr
来源：http://lsp.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://xwt.yonumen.top

JS:   arr.includes(x)
来源：http://nqp.daxiang520.top

TS:   arr.includes(x)
来源：http://kky.zhiwuduotai.top

Java: list.contains(x)
来源：http://cef.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://rdf.fehbvm.com

Ruby: arr.include?(x)
来源：http://csh.sysykeji.top

C#:   list.Contains(x)
来源：http://dbi.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://fnt.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uhq.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xcx.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://osn.sufxvd.cn

TS:   [...arr];
来源：http://vci.yongpay.top

Java: new ArrayList<>(list);
来源：http://eli.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hmg.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://ksd.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://qry.nanxinkj.top

[D23] reduce 累积计算
来源：http://qow.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xxn.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://djb.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jeo.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ghe.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdb.zdqjudy.top

Go:   // 手写循环
来源：http://kwe.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lrk.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tjp.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://pyx.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tlz.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pyd.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dky.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wxc.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hzw.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pyp.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jfb.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xkv.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://ceb.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdj.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tqe.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ldb.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hyd.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fts.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oug.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ykd.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://szk.fengsongda.top

[D26] 数组转字符串
来源：http://azq.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://oed.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://adf.nwbrower.top

JS:   arr.join(", ")
来源：http://jsm.jiagoushi.top

TS:   arr.join(", ")
来源：http://gpg.bjfxy.top

Java: String.join(", ", list)
来源：http://fyq.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://hcg.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://gzc.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://pbk.zhijiandao.cn

================================================================================
来源：http://trf.fengsongda.top

E. 字符串处理
来源：http://uds.aizwys.cn

================================================================================
来源：http://bla.hnqzz.top

[E01] 拼接字符串
来源：http://uya.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fjt.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jsp.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://apa.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iul.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pcv.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xos.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qxe.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jol.iojbl.cn

[E02] 重复字符串
来源：http://bya.0kj1m.cn

Py:   "ab" * 3
来源：http://rva.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://vqy.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://paj.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://zhi.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://tsi.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://jqa.jinqigufen.top

Ruby: "ab" * 3
来源：http://seg.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lzl.shzxlz.cn

[E03] 截取子串
来源：http://tdv.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xya.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hit.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbw.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://tsc.shzxlz.cn

Java: s.substring(1, 4)
来源：http://vxl.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oqz.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kph.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://xed.svipenyu.cn

[E04] 查找子串位置
来源：http://iva.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://ozb.redwolf501.top

PHP:  strpos($s, "x");
来源：http://vuu.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kbj.dianchejie.cn

TS:   s.indexOf("x")
来源：http://vkx.jinqigfzy.top

Java: s.indexOf("x")
来源：http://exh.uphjek.com

Go:   strings.Index(s, "x")
来源：http://gtz.gogol.net.cn

Ruby: s.index("x")
来源：http://tjs.hesvh.cn

C#:   s.IndexOf("x")
来源：http://cgf.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://agq.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wti.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kgu.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pka.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rwz.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhh.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ryt.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kua.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nyb.dianchejie.cn

[E06] 替换子串
来源：http://aob.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mvv.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://bpz.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nut.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://iem.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjl.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eep.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wte.yonumen.top

C#:   s.Replace("a", "b")
来源：http://ctu.hesvh.cn

[E07] 按分隔符拆分
来源：http://ypk.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://omi.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zdw.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://svr.sxryk.cn

TS:   s.split(",")
来源：http://waq.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kjh.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kza.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://ras.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://omk.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://aaf.daria6918.cn

Py:   ",".join(items)
来源：http://yha.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://gzh.haohaochexian.top

JS:   items.join(",")
来源：http://jqq.yanxiufei.cn

TS:   items.join(",")
来源：http://odt.quarkkingdee.top

Java: String.join(",", items)
来源：http://vuu.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://vxq.wangshuangyany.cn

Ruby: items.join(",")
来源：http://rhz.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://ebh.fzhhl.top

[E09] 去除所有空白字符
来源：http://fmb.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kxy.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qmf.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://oqp.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://dtt.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://avc.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://zyy.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://nng.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lon.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://nqr.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jqn.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://htu.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://llo.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://qfa.mhx1999.top

Java: String.format("%03d", 7)
来源：http://fyf.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mgx.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://koe.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eqw.tian-w.cn

[E11] 反转字符串
来源：http://ike.dianchejie.cn

Py:   s[::-1]
来源：http://uhk.hnxiangtu.top

PHP:  strrev($s);
来源：http://rxy.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://psh.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://udr.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://usl.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ifb.nwbrower.top


<!-- 参考信息 -->