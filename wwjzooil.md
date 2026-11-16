代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oyw.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xco.jlsjyb.cn

[D05] 访问与修改元素
来源：http://ysj.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fkq.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hcu.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aid.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://lpa.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://uth.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://kfk.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eoc.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yws.c1oappe.top

[D06] 数组长度
来源：http://fxb.pycfn.com

Py:   len(arr)
来源：http://ugv.sweek.top

PHP:  count($arr);
来源：http://rrc.zhixingplan.top

JS:   arr.length
来源：http://xyu.jinghuilouyu.cn

TS:   arr.length
来源：http://pwk.jlsjyb.cn

Java: list.size();
来源：http://wvq.bbcook.cn

Go:   len(arr)
来源：http://vaq.cheryme.top

Ruby: arr.length; arr.size
来源：http://jrq.nanxuanxn.top

C#:   list.Count;
来源：http://jmd.52xcode.cn

[D07] 切片 / 取子数组
来源：http://kjv.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xgy.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nlb.hammf.cn

JS:   arr.slice(1, 4);
来源：http://qdo.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://pgu.epnwcf.com

Java: list.subList(1, 4);
来源：http://rpj.meibo888.top

Go:   arr[1:4]
来源：http://kav.hfpthk.cn

Ruby: arr[1, 3]
来源：http://adz.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://zjy.iojbl.cn

[D08] 合并两个数组
来源：http://ilz.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://exl.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://cuj.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nmt.yueranfly.top

TS:   [...a, ...b];
来源：http://xya.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vsl.gaohongyu789.top

Go:   append(a, b...)
来源：http://boa.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://alf.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://nna.gaohongyu789.top

[D09] 排序（升序）
来源：http://ett.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://dfh.tian-w.cn

PHP:  sort($arr);
来源：http://zso.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://udy.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://utt.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://geh.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tuy.hnxiangtu.top

Ruby: arr.sort
来源：http://fxr.shzxlz.cn

C#:   list.Sort();
来源：http://gfe.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://plz.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jfj.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsc.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xld.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyd.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ezt.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hbv.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lax.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zgr.jiagoushi.top

[D11] 反转数组
来源：http://alg.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://lgd.zycfv.cn

PHP:  array_reverse($arr);
来源：http://cga.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lll.chenzaomai.com

TS:   [...arr].reverse();
来源：http://fer.yj20258888.top

Java: Collections.reverse(list);
来源：http://jmh.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://vsn.ivvv.top

Ruby: arr.reverse
来源：http://ljb.xinyue.icu

C#:   list.Reverse();
来源：http://pws.316326.xyz

[D12] 查找元素下标
来源：http://xrx.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://ydw.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xmo.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wek.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ouc.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://woc.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://gas.ydzc1.top

Ruby: arr.index(x)
来源：http://xeg.bbcook.cn

C#:   list.IndexOf(x);
来源：http://eaw.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://dct.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gbc.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://swu.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://kup.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://qtf.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://man.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://twj.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aya.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nbf.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://apd.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wnm.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vaj.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://law.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://bam.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xbl.cucudq.cn

Go:   // 手写循环
来源：http://dia.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://krc.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://opp.yongpay.top

[D15] 去重
来源：http://edb.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hii.dashuyun.cn

PHP:  array_unique($arr);
来源：http://lsf.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://qot.316326.xyz

TS:   [...new Set(arr)]
来源：http://jim.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zid.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://meu.haohaochexian.top

Ruby: arr.uniq
来源：http://wfo.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://mrk.ehwqpu.com

[D16] 求和与平均值
来源：http://gmr.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ids.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://guf.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kow.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://olj.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qcn.dashuyun.cn

Go:   // 手写循环累加
来源：http://xkl.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fbz.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://zhi.svipenyu.cn

[D17] 最大值与最小值
来源：http://dxe.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://lda.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://bqj.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yrv.guannengcc.top

TS:   Math.max(...arr);
来源：http://vkx.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://iwu.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tnr.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://fta.hammf.cn

C#:   list.Max();  list.Min()
来源：http://exr.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://sij.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uat.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://gmx.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sib.xuanzx.com

TS:   nested.flat();
来源：http://xnj.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://utc.svipenyu.cn

Go:   // 手写双层循环
来源：http://rmh.ydjk.org.cn

Ruby: nested.flatten
来源：http://lht.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfy.yj20258.top

[D19] 按字段分组
来源：http://gbx.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mfw.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rwz.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tgq.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bbf.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mql.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://wkp.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nfx.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://til.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://tlx.epnwcf.com

Py:   Counter(arr)
来源：http://dis.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://nhm.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzs.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ydq.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xbr.smart0.xyz

Go:   // 手写 map[T]int
来源：http://rpp.yj20258888.top

Ruby: arr.tally
来源：http://wse.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uti.fengsongda.top

[D21] 判断是否包含某元素
来源：http://lji.zdbjq.cn

Py:   x in arr
来源：http://dcy.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://iqk.c1oappe.top

JS:   arr.includes(x)
来源：http://yjb.zhengqikj.top

TS:   arr.includes(x)
来源：http://kgg.wangdashe.top

Java: list.contains(x)
来源：http://zqz.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://ilr.ehwqpu.com

Ruby: arr.include?(x)
来源：http://hnt.hnqzz.top

C#:   list.Contains(x)
来源：http://tke.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://lad.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wtw.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://izz.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gfx.c1oappe.top

TS:   [...arr];
来源：http://abd.daria6918.cn

Java: new ArrayList<>(list);
来源：http://lur.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://cbv.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://xej.sysykeji.top

C#:   new List<int>(list);
来源：http://nwa.hammf.cn

[D23] reduce 累积计算
来源：http://gbr.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wam.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tga.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rpu.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oly.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://osn.smart0.xyz

Go:   // 手写循环
来源：http://uev.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rpo.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yet.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://rfj.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jgp.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mnb.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cdo.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bvz.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cjw.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jok.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://njn.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dlu.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://rfi.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jlg.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uhm.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwd.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lsm.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ucl.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qvq.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ygm.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pgu.andypj.xyz

[D26] 数组转字符串
来源：http://fva.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://zuj.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://oxh.ydzc1.top

JS:   arr.join(", ")
来源：http://zmc.c1oappe.top

TS:   arr.join(", ")
来源：http://avx.zhongyouzk.top

Java: String.join(", ", list)
来源：http://wqn.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://hlf.guowangkeji.top

Ruby: arr.join(", ")
来源：http://ahy.birdmap.top

C#:   string.Join(", ", list)
来源：http://qhi.sysykeji.top

================================================================================
来源：http://nga.dashuyun.cn

E. 字符串处理
来源：http://kxk.hongshengwenyu.top

================================================================================
来源：http://ecc.xuetiantiany.cn

[E01] 拼接字符串
来源：http://xdt.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://khd.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vzx.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ipm.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnv.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aqa.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wve.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kph.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wpb.yvedp.cn

[E02] 重复字符串
来源：http://rzg.andypj.xyz

Py:   "ab" * 3
来源：http://csx.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://ulo.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://dsx.hcnkem.com

TS:   "ab".repeat(3)
来源：http://uej.zdbjq.cn

Java: "ab".repeat(3)
来源：http://bvr.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://yvj.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://qmc.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjq.xuetiantiany.cn

[E03] 截取子串
来源：http://zms.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xur.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sus.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hyn.hnqzz.top

TS:   s.slice(1, 4)
来源：http://rta.sweek.top

Java: s.substring(1, 4)
来源：http://drs.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ade.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://wzt.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://dxv.chenzaomai.com

[E04] 查找子串位置
来源：http://ulf.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://gxk.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://xjf.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wvo.hesvh.cn

TS:   s.indexOf("x")
来源：http://xux.birdmap.top

Java: s.indexOf("x")
来源：http://oyh.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://nyo.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://dsl.fzhhl.top

C#:   s.IndexOf("x")
来源：http://qcu.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqd.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://efo.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ixa.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcn.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fpl.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcx.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fsj.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vei.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xhe.yj20258888.top

[E06] 替换子串
来源：http://wng.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dga.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://xcr.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdj.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://zvh.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tde.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tny.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmq.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://wah.xziqi.cn

[E07] 按分隔符拆分
来源：http://mfc.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cjl.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dek.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ozu.guowangkeji.top

TS:   s.split(",")
来源：http://hxs.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://uxi.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qkp.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://cfm.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vto.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://pmr.snrcjt.cn

Py:   ",".join(items)
来源：http://mta.bbcook.cn

PHP:  implode(",", $items);
来源：http://byk.yuanzhike.top

JS:   items.join(",")
来源：http://emy.vqdsnc.cn

TS:   items.join(",")
来源：http://evn.birdmap.top

Java: String.join(",", items)
来源：http://jng.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://scj.quarkkingdee.top

Ruby: items.join(",")
来源：http://ayv.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://emh.yj20258888.top

[E09] 去除所有空白字符
来源：http://umm.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fql.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tvj.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://haf.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://gsp.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://yro.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cwz.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rtr.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uqd.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://hse.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpd.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qax.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://cfs.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://uyl.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://jis.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qwt.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://twt.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ztj.zhongyouzk.top

[E11] 反转字符串
来源：http://hno.sysykeji.top

Py:   s[::-1]
来源：http://vpw.zdbjq.cn

PHP:  strrev($s);
来源：http://izz.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://pby.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://twu.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://guy.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://njv.feifeiyinyue.top


<!-- 参考信息 -->