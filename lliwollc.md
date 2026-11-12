代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cso.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gzq.chenzaomai.com

[D05] 访问与修改元素
来源：http://lqo.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bia.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bhk.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qkv.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://qhf.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://zsl.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://jxd.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfb.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vxf.ydzc1.top

[D06] 数组长度
来源：http://nrv.yuxming.cn

Py:   len(arr)
来源：http://oqw.mhx1999.top

PHP:  count($arr);
来源：http://dcs.316326.xyz

JS:   arr.length
来源：http://hji.vqdsnc.cn

TS:   arr.length
来源：http://fpc.fengsongda.top

Java: list.size();
来源：http://yfm.xuanzx.com

Go:   len(arr)
来源：http://orx.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://gve.jiagoushi.top

C#:   list.Count;
来源：http://nfx.xinyue.icu

[D07] 切片 / 取子数组
来源：http://atj.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bvb.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oaj.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://yag.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://nar.uphjek.com

Java: list.subList(1, 4);
来源：http://ttf.yanxiufei.cn

Go:   arr[1:4]
来源：http://enc.316326.xyz

Ruby: arr[1, 3]
来源：http://yfr.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://yxf.ivvv.top

[D08] 合并两个数组
来源：http://mtd.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://skl.tanke756.top

PHP:  array_merge($a, $b);
来源：http://etn.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bfv.sysykeji.top

TS:   [...a, ...b];
来源：http://mlw.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nsf.xinyue.icu

Go:   append(a, b...)
来源：http://nno.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://frf.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://fsf.hfpthk.cn

[D09] 排序（升序）
来源：http://yak.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://chs.zdbjq.cn

PHP:  sort($arr);
来源：http://ehg.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://prq.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://irk.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yvl.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eeq.jlsjyb.cn

Ruby: arr.sort
来源：http://rmu.xinyue.icu

C#:   list.Sort();
来源：http://efl.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ind.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://odx.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qlo.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjn.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfy.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://utr.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uuw.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fnu.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xeg.jqgufenzy.top

[D11] 反转数组
来源：http://skk.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://hnm.yfazqb.com

PHP:  array_reverse($arr);
来源：http://twq.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sch.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://pqh.sxryk.cn

Java: Collections.reverse(list);
来源：http://dmb.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://djh.zdbjq.cn

Ruby: arr.reverse
来源：http://whe.zdbjq.cn

C#:   list.Reverse();
来源：http://iiw.tarul.cn

[D12] 查找元素下标
来源：http://dwd.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://kzj.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rmp.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ppn.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kbo.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vwo.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://hwp.c1oappe.top

Ruby: arr.index(x)
来源：http://jsz.yuxming.cn

C#:   list.IndexOf(x);
来源：http://ykj.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://ouq.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ulw.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cex.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://zaq.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://lzq.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ezs.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hly.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ptj.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://uju.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://hvl.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wzc.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://evr.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://vbx.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://fnd.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rnk.vqdsnc.cn

Go:   // 手写循环
来源：http://aqa.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://uji.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xyn.meibo888.top

[D15] 去重
来源：http://xej.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwl.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://idk.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://ojx.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://oaf.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sly.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://csl.cheryme.top

Ruby: arr.uniq
来源：http://mel.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://hnr.zhengqikj.top

[D16] 求和与平均值
来源：http://lni.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tyf.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jdx.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jku.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vqr.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fld.hfpthk.cn

Go:   // 手写循环累加
来源：http://ahj.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hji.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://uyh.uphjek.com

[D17] 最大值与最小值
来源：http://zml.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://kfq.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://uav.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://swi.ydzc1.top

TS:   Math.max(...arr);
来源：http://pzv.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iac.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ryg.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://hgu.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://jao.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://xym.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mlc.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://ves.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tuf.tianlin.xyz

TS:   nested.flat();
来源：http://omb.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://poi.yanxiufei.cn

Go:   // 手写双层循环
来源：http://nzu.zhijiandao.cn

Ruby: nested.flatten
来源：http://xol.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://amu.zhengqikj.top

[D19] 按字段分组
来源：http://iba.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tbf.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://son.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eft.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fjh.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pth.yonumen.top

Go:   // 手写 map[string][]T
来源：http://fwg.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wwy.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aub.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://crm.jinqigufen.top

Py:   Counter(arr)
来源：http://ypx.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://cdo.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://slm.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://saj.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mbf.tarul.cn

Go:   // 手写 map[T]int
来源：http://byy.yj20258888.top

Ruby: arr.tally
来源：http://nso.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fwr.52xcode.cn

[D21] 判断是否包含某元素
来源：http://nle.52xcode.cn

Py:   x in arr
来源：http://qwd.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://ksi.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://snp.cucudq.cn

TS:   arr.includes(x)
来源：http://lsa.dianchejie.cn

Java: list.contains(x)
来源：http://apy.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://keu.snrcjt.cn

Ruby: arr.include?(x)
来源：http://sbu.zhongyouzk.top

C#:   list.Contains(x)
来源：http://moq.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://wff.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zet.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ivf.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sru.zhijiandao.cn

TS:   [...arr];
来源：http://rxu.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://fpm.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://bfu.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://bai.cheryme.top

C#:   new List<int>(list);
来源：http://rmm.dashuyun.cn

[D23] reduce 累积计算
来源：http://ncs.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ska.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uow.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aul.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffa.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ldn.ehwqpu.com

Go:   // 手写循环
来源：http://ehp.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aww.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rcn.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://bxj.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://chh.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzk.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nsy.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ihq.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blg.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xtq.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dlv.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dvg.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://mil.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://poi.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fug.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vtn.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kvg.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://som.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kov.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://itn.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sbm.316326.xyz

[D26] 数组转字符串
来源：http://vle.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://zpy.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://kwc.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://ing.316326.xyz

TS:   arr.join(", ")
来源：http://qpt.tian-w.cn

Java: String.join(", ", list)
来源：http://qht.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://ncw.0kj1m.cn

Ruby: arr.join(", ")
来源：http://upg.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://ozu.hfpthk.cn

================================================================================
来源：http://mcw.xuetiantiany.cn

E. 字符串处理
来源：http://hcz.ydjk.org.cn

================================================================================
来源：http://gtp.yongpay.top

[E01] 拼接字符串
来源：http://yya.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://anh.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cfj.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oqj.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fzs.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wnu.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gga.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qwy.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xcf.chenlongwang.top

[E02] 重复字符串
来源：http://xrz.jiagoushi.top

Py:   "ab" * 3
来源：http://tgk.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://dmk.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://tii.epnwcf.com

TS:   "ab".repeat(3)
来源：http://qku.yueranfly.top

Java: "ab".repeat(3)
来源：http://pgf.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dxb.52xcode.cn

Ruby: "ab" * 3
来源：http://fwt.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iit.sjlbkw.cn

[E03] 截取子串
来源：http://haj.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fci.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gqy.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hbw.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://uml.svipenyu.cn

Java: s.substring(1, 4)
来源：http://sos.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mqj.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://omu.316326.xyz

C#:   s.Substring(1, 3)
来源：http://jfc.nanxuanxn.top

[E04] 查找子串位置
来源：http://qfw.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://ivn.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://ugh.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dgd.tanke756.top

TS:   s.indexOf("x")
来源：http://cgf.haohaochexian.top

Java: s.indexOf("x")
来源：http://lkr.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://xxn.kuanghao11.cn

Ruby: s.index("x")
来源：http://jem.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://ryp.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://egi.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://onv.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ipo.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oan.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ijq.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://faa.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cxt.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://les.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://esl.zdbjq.cn

[E06] 替换子串
来源：http://zzc.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gdh.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://whu.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktg.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://rnm.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pku.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xgo.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zym.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://ntw.chenlongwang.top

[E07] 按分隔符拆分
来源：http://uah.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://inz.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yoe.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qfe.shzxlz.cn

TS:   s.split(",")
来源：http://sbx.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eew.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vdr.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://pzr.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ofv.yueranfly.top

[E08] 数组按分隔符合并
来源：http://wdp.xinyue.icu

Py:   ",".join(items)
来源：http://qxv.zdqjudy.top

PHP:  implode(",", $items);
来源：http://soj.mhx1999.top

JS:   items.join(",")
来源：http://uez.xziqi.cn

TS:   items.join(",")
来源：http://qtc.zdbjq.cn

Java: String.join(",", items)
来源：http://sen.yongpay.top

Go:   strings.Join(items, ",")
来源：http://fsq.ctjpmb.com

Ruby: items.join(",")
来源：http://gpt.cucudq.cn

C#:   string.Join(",", items)
来源：http://lbd.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://oah.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ffw.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kbk.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://gob.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://fum.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://szo.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://etn.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://jud.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xjs.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://jlq.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pgk.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ujn.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://vwv.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://kft.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://ndg.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mwr.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://huz.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uff.sufxvd.cn

[E11] 反转字符串
来源：http://dmh.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://xxq.yongpay.top

PHP:  strrev($s);
来源：http://vjl.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://qzp.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://npn.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ezr.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tlu.jinqigfzy.top


<!-- 参考信息 -->