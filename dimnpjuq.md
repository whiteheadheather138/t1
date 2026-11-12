代发 wailian999

[D07] 切片 / 取子数组
来源：http://all.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axx.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tnv.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://jkr.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://idk.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://pgf.shuidangran.top

Go:   arr[1:4]
来源：http://ulq.fzhhl.top

Ruby: arr[1, 3]
来源：http://gci.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://tba.yuxming.cn

[D08] 合并两个数组
来源：http://klk.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://aiq.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://qgj.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lzf.fehbvm.com

TS:   [...a, ...b];
来源：http://aza.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rye.tianlin.xyz

Go:   append(a, b...)
来源：http://nlh.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://joq.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://nwk.xylfe.cn

[D09] 排序（升序）
来源：http://ncg.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://roo.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://ezs.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zel.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://syw.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://rih.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bmj.epnwcf.com

Ruby: arr.sort
来源：http://bbt.uphjek.com

C#:   list.Sort();
来源：http://yuh.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://not.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ruz.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpt.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ftw.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jym.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ebk.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qal.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yrw.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kdt.hongshengwenyu.top

[D11] 反转数组
来源：http://klh.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ywo.316326.xyz

PHP:  array_reverse($arr);
来源：http://dks.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tcm.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://vsv.gzhubu.top

Java: Collections.reverse(list);
来源：http://qfy.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://gge.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://tie.zdbjq.cn

C#:   list.Reverse();
来源：http://rax.guowangkeji.top

[D12] 查找元素下标
来源：http://vfc.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://ywy.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kaq.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fen.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dip.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uql.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://tpv.vehdjk.com

Ruby: arr.index(x)
来源：http://wux.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://ghm.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://fok.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cqo.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cwb.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://vgy.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://frj.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zmv.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ybg.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uri.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hhw.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://jka.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://chv.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://byj.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://gmn.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://nmp.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hmm.52xcode.cn

Go:   // 手写循环
来源：http://zci.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sts.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lhz.daria6918.cn

[D15] 去重
来源：http://nbv.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hww.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://ibl.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://flo.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://vpy.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vmd.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kep.zhengqikj.top

Ruby: arr.uniq
来源：http://iml.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://dua.hongshengwenyu.top

[D16] 求和与平均值
来源：http://exh.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xty.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ghk.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gmp.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvo.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kdr.vqdsnc.cn

Go:   // 手写循环累加
来源：http://mcn.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://leu.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://xpf.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://rzq.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://wtd.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://pla.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xqi.sysykeji.top

TS:   Math.max(...arr);
来源：http://hak.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://ybo.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ccr.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://ima.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://ozz.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://giq.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zfr.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://gvl.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lcj.svipenyu.cn

TS:   nested.flat();
来源：http://uhk.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mcs.sysykeji.top

Go:   // 手写双层循环
来源：http://esc.epnwcf.com

Ruby: nested.flatten
来源：http://ssq.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ngx.aizwys.cn

[D19] 按字段分组
来源：http://gvt.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qjm.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zbf.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpa.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vps.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pef.hammf.cn

Go:   // 手写 map[string][]T
来源：http://xaq.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ddy.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eqc.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://fsx.hysaishi.cn

Py:   Counter(arr)
来源：http://xik.hesvh.cn

PHP:  array_count_values($arr);
来源：http://srj.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://brp.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzo.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awc.tarul.cn

Go:   // 手写 map[T]int
来源：http://tcv.jlsjyb.cn

Ruby: arr.tally
来源：http://oyh.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lri.tarul.cn

[D21] 判断是否包含某元素
来源：http://ufb.ctjpmb.com

Py:   x in arr
来源：http://ivm.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://wup.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://nfx.birdmap.top

TS:   arr.includes(x)
来源：http://cep.sjlbkw.cn

Java: list.contains(x)
来源：http://pyx.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://tnw.nwbrower.top

Ruby: arr.include?(x)
来源：http://kas.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://ipp.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://gkp.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mok.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://din.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ccp.zdqjudy.top

TS:   [...arr];
来源：http://lpr.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://zsh.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://obb.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://dhs.ydjk.org.cn

C#:   new List<int>(list);
来源：http://nom.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://upu.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvt.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lal.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jio.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nul.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gnj.sxryk.cn

Go:   // 手写循环
来源：http://lpp.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dqj.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://szz.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://hsg.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ocr.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpy.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qmu.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qmg.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uzj.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ski.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bjj.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zps.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://zbl.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oaa.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbw.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jil.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jfy.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ipr.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mbt.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zmo.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://afd.ydzc1.top

[D26] 数组转字符串
来源：http://cxx.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://ohc.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://twp.zhijiandao.cn

JS:   arr.join(", ")
来源：http://bea.xziqi.cn

TS:   arr.join(", ")
来源：http://swu.shzxlz.cn

Java: String.join(", ", list)
来源：http://qqd.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://lai.tian-w.cn

Ruby: arr.join(", ")
来源：http://ett.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://wnt.yj202588.top

================================================================================
来源：http://dpn.hysaishi.cn

E. 字符串处理
来源：http://pfc.hnqzz.top

================================================================================
来源：http://pni.chenzaomai.com

[E01] 拼接字符串
来源：http://jcp.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nem.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lif.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jol.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tpg.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lix.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikv.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wvw.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rmk.yangfankeji.com

[E02] 重复字符串
来源：http://kmr.shangyingyoupin.top

Py:   "ab" * 3
来源：http://afe.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://mxx.xuanzx.com

JS:   "ab".repeat(3)
来源：http://ahi.wangdashe.top

TS:   "ab".repeat(3)
来源：http://xpm.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://bqw.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://iux.jqgfzy.top

Ruby: "ab" * 3
来源：http://usx.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ekz.shangyingyoupin.top

[E03] 截取子串
来源：http://zcm.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gge.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nus.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://naj.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://lpg.ivvv.top

Java: s.substring(1, 4)
来源：http://kep.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mpx.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xyd.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://fsu.hysaishi.cn

[E04] 查找子串位置
来源：http://hfe.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://ylz.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://teg.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yhe.daria6918.cn

TS:   s.indexOf("x")
来源：http://dal.epnwcf.com

Java: s.indexOf("x")
来源：http://xcq.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://ayi.yuanzhike.top

Ruby: s.index("x")
来源：http://wnv.yj20258888.top

C#:   s.IndexOf("x")
来源：http://wwi.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://aot.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tdc.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dgq.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ujt.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rwv.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vkm.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uih.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ryr.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqa.52xcode.cn

[E06] 替换子串
来源：http://mlq.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nry.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://jfa.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vet.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://whm.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqw.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://syj.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://agr.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://kof.nanxinkj.top

[E07] 按分隔符拆分
来源：http://bue.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://liv.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ofk.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebo.yangfankeji.com

TS:   s.split(",")
来源：http://vyi.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nie.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ifw.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://ynq.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sao.tian-w.cn

[E08] 数组按分隔符合并
来源：http://zog.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://jea.sweek.top

PHP:  implode(",", $items);
来源：http://wtm.vehdjk.com

JS:   items.join(",")
来源：http://vwd.hesvh.cn

TS:   items.join(",")
来源：http://zro.jqgufenzy.top

Java: String.join(",", items)
来源：http://uui.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://ayk.daria6918.cn

Ruby: items.join(",")
来源：http://cgf.yonumen.top

C#:   string.Join(",", items)
来源：http://yrf.hysaishi.cn

[E09] 去除所有空白字符
来源：http://drx.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pwg.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mbm.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://xez.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://uuf.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://dry.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ugp.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://fhr.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbc.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://awx.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://phk.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zxc.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://jop.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://mhu.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://kgy.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tuf.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abt.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xxt.xuanzx.com

[E11] 反转字符串
来源：http://eir.xuanzx.com

Py:   s[::-1]
来源：http://gco.nwbrower.top

PHP:  strrev($s);
来源：http://rwp.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://qpt.sweek.top

TS:   [...s].reverse().join("")
来源：http://tns.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://lgk.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wcx.ydjk.org.cn

Ruby: s.reverse
来源：http://ork.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ftj.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://jxx.quarkkingdee.top

Py:   s.count("a")
来源：http://jjy.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://rtb.yfazqb.com

JS:   s.split("a").length - 1
来源：http://cnk.yonumen.top

TS:   s.split("a").length - 1
来源：http://pra.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jem.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://ycf.chenjidiqi.icu

Ruby: s.count("a")
来源：http://wem.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://sye.nwbrower.top

[E13] 逐字符遍历
来源：http://bpi.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://kkn.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xkd.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://dnl.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zro.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xhp.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vjd.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rok.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fce.xziqi.cn


<!-- 参考信息 -->