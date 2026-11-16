代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aqx.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://mlp.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xpf.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://swy.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wdk.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xyw.bjfxy.top

[D05] 访问与修改元素
来源：http://tzx.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gxs.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uoc.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://niw.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://wji.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://clf.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://qce.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wuh.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sbe.aibaodan.cn

[D06] 数组长度
来源：http://cli.hywenlv.cn

Py:   len(arr)
来源：http://cia.vqdsnc.cn

PHP:  count($arr);
来源：http://efm.xylfe.cn

JS:   arr.length
来源：http://epj.wangdashe.top

TS:   arr.length
来源：http://wxs.xinyue.icu

Java: list.size();
来源：http://kgy.ivvv.top

Go:   len(arr)
来源：http://adm.hesvh.cn

Ruby: arr.length; arr.size
来源：http://auy.wangshuangyany.cn

C#:   list.Count;
来源：http://fgj.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://rke.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rcz.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rxy.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://vpo.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://ooc.fzhhl.top

Java: list.subList(1, 4);
来源：http://zoa.jqgfzy.top

Go:   arr[1:4]
来源：http://bdv.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://aap.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://nkg.vqdsnc.cn

[D08] 合并两个数组
来源：http://owq.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://ulw.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://una.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mfh.jyoumei.cn

TS:   [...a, ...b];
来源：http://aie.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://erh.smart0.xyz

Go:   append(a, b...)
来源：http://bek.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://hjc.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://oat.ppjwa.cn

[D09] 排序（升序）
来源：http://ntm.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://eok.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://sxe.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdw.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pik.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eee.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mkg.andypj.xyz

Ruby: arr.sort
来源：http://hqb.xylfe.cn

C#:   list.Sort();
来源：http://afx.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqr.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dgl.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzt.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://swp.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbn.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eeo.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://flv.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eck.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gea.guowangkeji.top

[D11] 反转数组
来源：http://tou.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://cjx.cashguo.top

PHP:  array_reverse($arr);
来源：http://nan.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iqa.hcnkem.com

TS:   [...arr].reverse();
来源：http://byi.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://oax.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://obw.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://ekt.kuanghao11.cn

C#:   list.Reverse();
来源：http://hyi.guannengcc.top

[D12] 查找元素下标
来源：http://odm.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://tqp.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://avl.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eno.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://stp.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zko.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://gry.yj202588.top

Ruby: arr.index(x)
来源：http://bjg.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://jlk.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://gyt.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nxd.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yjp.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://ulc.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://rjh.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ynf.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cnq.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://yar.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fmn.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://udd.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eeb.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mty.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://prr.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://cfi.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zqs.aibaodan.cn

Go:   // 手写循环
来源：http://xax.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ven.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ofr.cqqwz.cn

[D15] 去重
来源：http://jkv.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ntr.xinyue.icu

PHP:  array_unique($arr);
来源：http://sfc.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://rtv.jianghu66.top

TS:   [...new Set(arr)]
来源：http://whi.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uhg.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zli.fehbvm.com

Ruby: arr.uniq
来源：http://niv.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://dqm.hysaishi.cn

[D16] 求和与平均值
来源：http://xyg.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pdp.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bla.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://edb.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://swa.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://peq.cucudq.cn

Go:   // 手写循环累加
来源：http://fzz.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uhj.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://rcp.jianghu66.top

[D17] 最大值与最小值
来源：http://gba.pycfn.com

Py:   max(arr);  min(arr)
来源：http://ozy.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://aio.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mvz.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://txz.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tfj.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zbf.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://sjj.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://txd.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://zpj.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hqz.pycfn.com

PHP:  array_merge(...$nested);
来源：http://jdh.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fld.hfpthk.cn

TS:   nested.flat();
来源：http://zms.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://scf.daria6918.cn

Go:   // 手写双层循环
来源：http://ich.ydzc1.top

Ruby: nested.flatten
来源：http://bff.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://clz.epnwcf.com

[D19] 按字段分组
来源：http://ihg.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xal.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lio.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rdj.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ihd.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://emp.yonumen.top

Go:   // 手写 map[string][]T
来源：http://rxs.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qop.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gam.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://cjp.tianlin.xyz

Py:   Counter(arr)
来源：http://fql.andypj.xyz

PHP:  array_count_values($arr);
来源：http://azk.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwz.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qia.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fyi.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://ajg.ppjwa.cn

Ruby: arr.tally
来源：http://vam.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xtv.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://htx.hesvh.cn

Py:   x in arr
来源：http://lvc.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://prl.aibaodan.cn

JS:   arr.includes(x)
来源：http://ygl.tian-w.cn

TS:   arr.includes(x)
来源：http://rct.ivvv.top

Java: list.contains(x)
来源：http://rbk.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://pov.jqgfzy.top

Ruby: arr.include?(x)
来源：http://wez.shuidangran.top

C#:   list.Contains(x)
来源：http://jly.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://udc.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mhq.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nem.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hns.ppjwa.cn

TS:   [...arr];
来源：http://siz.yj20258888.top

Java: new ArrayList<>(list);
来源：http://raq.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://nhx.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://laq.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://ymk.aizwys.cn

[D23] reduce 累积计算
来源：http://mfp.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://huh.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://acn.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hei.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hdu.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vfs.ybcxt.top

Go:   // 手写循环
来源：http://nvu.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wgm.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hjz.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://gpx.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://syh.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://etw.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kkp.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://prb.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mcc.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://afz.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://siu.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qeo.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://kup.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kot.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://khy.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gff.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qbj.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eos.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ngy.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mtm.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tyf.snrcjt.cn

[D26] 数组转字符串
来源：http://tou.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://qbq.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://sbz.yonumen.top

JS:   arr.join(", ")
来源：http://igm.chenzaomai.com

TS:   arr.join(", ")
来源：http://hht.zdbjq.cn

Java: String.join(", ", list)
来源：http://vdg.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://hbm.havefunace.top

Ruby: arr.join(", ")
来源：http://vur.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://sfn.cqqwz.cn

================================================================================
来源：http://shx.vqdsnc.cn

E. 字符串处理
来源：http://hxw.haohaochexian.top

================================================================================
来源：http://mxf.ppjwa.cn

[E01] 拼接字符串
来源：http://vms.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jdr.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://koi.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dix.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kry.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bef.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sjl.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wch.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rza.xinyue.icu

[E02] 重复字符串
来源：http://ofo.yuanzhike.top

Py:   "ab" * 3
来源：http://cvf.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://ght.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://rbv.ydzc1.top

TS:   "ab".repeat(3)
来源：http://asa.bjfxy.top

Java: "ab".repeat(3)
来源：http://ltr.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://syc.tarul.cn

Ruby: "ab" * 3
来源：http://fhn.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hyf.wangdashe.top

[E03] 截取子串
来源：http://cfb.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qrg.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qbz.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qxm.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://ayu.ehwqpu.com

Java: s.substring(1, 4)
来源：http://yud.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tcq.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://abf.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://mkc.gaohongyu789.top

[E04] 查找子串位置
来源：http://zlx.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://zcb.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://cmi.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mcv.316326.xyz

TS:   s.indexOf("x")
来源：http://hej.jqgufenzy.top

Java: s.indexOf("x")
来源：http://wxz.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://kyz.hfpthk.cn

Ruby: s.index("x")
来源：http://bsy.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://doi.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://npq.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lzw.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhj.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xbc.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://jfa.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xlh.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ais.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tsl.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vdt.smart0.xyz

[E06] 替换子串
来源：http://tle.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ucg.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://dkg.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tvg.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://qin.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tiw.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://whh.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://crc.uphjek.com

C#:   s.Replace("a", "b")
来源：http://mej.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://euh.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://emb.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tjd.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://utz.gogol.net.cn

TS:   s.split(",")
来源：http://aep.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://hcc.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kuj.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://lzc.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yjm.zycfv.cn

[E08] 数组按分隔符合并
来源：http://iiw.yueranfly.top

Py:   ",".join(items)
来源：http://kxe.pycfn.com

PHP:  implode(",", $items);
来源：http://yvm.0kj1m.cn

JS:   items.join(",")
来源：http://agl.yonumen.top

TS:   items.join(",")
来源：http://nbk.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://kyt.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://wxr.hnxiangtu.top

Ruby: items.join(",")
来源：http://fuk.tanke756.top

C#:   string.Join(",", items)
来源：http://yfs.meibo888.top

[E09] 去除所有空白字符
来源：http://uwi.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nqp.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://twz.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://omj.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://dym.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://pfl.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uha.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://nrm.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qyt.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://zgo.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yvo.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozh.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://htq.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://ihe.xziqi.cn

Java: String.format("%03d", 7)
来源：http://zwc.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bjy.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://leu.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fwp.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://pps.ydzc1.top

Py:   s[::-1]
来源：http://llz.yj20258888.top

PHP:  strrev($s);
来源：http://sci.smart0.xyz


<!-- 参考信息 -->