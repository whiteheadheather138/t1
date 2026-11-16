代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hsb.tanke756.top

[D04] 删除元素
来源：http://ltw.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oeo.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgn.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yvu.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://wbe.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mdr.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qvf.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jre.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hui.xinyue.icu

[D05] 访问与修改元素
来源：http://tkz.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://guu.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eir.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eih.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://mtk.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://nou.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://kll.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hjp.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wbt.gotoacloud.top

[D06] 数组长度
来源：http://efi.smart0.xyz

Py:   len(arr)
来源：http://ukf.fengsongda.top

PHP:  count($arr);
来源：http://wbk.ywan-chungtsiang.top

JS:   arr.length
来源：http://aqn.hesvh.cn

TS:   arr.length
来源：http://nql.jinqigfzy.top

Java: list.size();
来源：http://bko.ehwqpu.com

Go:   len(arr)
来源：http://fza.ybcxt.top

Ruby: arr.length; arr.size
来源：http://del.xylfe.cn

C#:   list.Count;
来源：http://sjl.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://oqs.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iwa.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sth.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://iju.birdmap.top

TS:   arr.slice(1, 4);
来源：http://qnv.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://cnw.pycfn.com

Go:   arr[1:4]
来源：http://kyd.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://utc.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://kfb.tanke756.top

[D08] 合并两个数组
来源：http://vvj.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://fxu.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://tiu.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rjs.yanxiufei.cn

TS:   [...a, ...b];
来源：http://pzq.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kke.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://rdg.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://znn.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://crd.fktsv.cn

[D09] 排序（升序）
来源：http://bfx.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://bga.birdmap.top

PHP:  sort($arr);
来源：http://xpy.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bcg.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rsb.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://oxm.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hky.hywenlv.cn

Ruby: arr.sort
来源：http://aui.pycfn.com

C#:   list.Sort();
来源：http://osv.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://auf.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://neq.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fle.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://byg.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://olr.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yuk.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uye.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nsp.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tnp.ehwqpu.com

[D11] 反转数组
来源：http://nbq.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://woe.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://ndh.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://usn.guowangkeji.top

TS:   [...arr].reverse();
来源：http://xff.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://pmh.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://epj.sxryk.cn

Ruby: arr.reverse
来源：http://koq.ppjwa.cn

C#:   list.Reverse();
来源：http://luy.jqgufenzy.top

[D12] 查找元素下标
来源：http://wrg.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://cli.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ncq.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vue.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pof.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqi.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://epv.gaohongyu789.top

Ruby: arr.index(x)
来源：http://cba.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://fxi.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://xbt.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hez.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbj.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://skd.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://acn.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lvi.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eue.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ooa.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zuc.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://cns.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hsf.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kzf.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://sgb.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://ppx.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fdh.vqdsnc.cn

Go:   // 手写循环
来源：http://zjt.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ayg.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jrp.yanxiufei.cn

[D15] 去重
来源：http://bxr.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jtx.cdnleiting.top

PHP:  array_unique($arr);
来源：http://gdi.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://ste.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://dvz.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ivp.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ltx.jqgufenzy.top

Ruby: arr.uniq
来源：http://pao.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://ztb.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://tjq.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yvz.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nay.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kyl.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzs.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tgg.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://dwm.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zyi.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://lar.shuidangran.top

[D17] 最大值与最小值
来源：http://ouk.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://ztd.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://zlv.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://evf.9152youxi.cn

TS:   Math.max(...arr);
来源：http://czw.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jtx.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xtm.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://afp.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://glz.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://ski.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xig.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://lgt.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kwe.chenjidiqi.icu

TS:   nested.flat();
来源：http://phw.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alj.yj202588.top

Go:   // 手写双层循环
来源：http://qhh.smart0.xyz

Ruby: nested.flatten
来源：http://lsg.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uux.yj202588.top

[D19] 按字段分组
来源：http://fwc.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fst.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://igy.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ykz.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://umc.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jeu.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://zvk.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ukk.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pzy.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://sbm.haohaochexian.top

Py:   Counter(arr)
来源：http://xgl.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://elh.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erg.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zlb.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pvx.aibaodan.cn

Go:   // 手写 map[T]int
来源：http://ajd.tarul.cn

Ruby: arr.tally
来源：http://elg.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvk.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://yoq.fktsv.cn

Py:   x in arr
来源：http://nzh.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://jrz.cashguo.top

JS:   arr.includes(x)
来源：http://gnv.fzhhl.top

TS:   arr.includes(x)
来源：http://ppu.ydzc1.top

Java: list.contains(x)
来源：http://tkl.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://ywh.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://pxh.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://ugl.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://jrm.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uoi.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wtx.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cat.uphjek.com

TS:   [...arr];
来源：http://iht.daxiang520.top

Java: new ArrayList<>(list);
来源：http://kup.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://wro.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://mww.dianchejie.cn

C#:   new List<int>(list);
来源：http://gpo.tanke756.top

[D23] reduce 累积计算
来源：http://tfy.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vbg.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://old.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qef.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyr.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kur.guowangkeji.top

Go:   // 手写循环
来源：http://olu.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dpr.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://egn.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://lxf.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zfl.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xzu.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mth.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kca.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xeh.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sdb.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hop.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vrb.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://ovw.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dhx.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dne.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yzx.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vsf.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hge.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vtp.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zfx.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bkr.sysykeji.top

[D26] 数组转字符串
来源：http://nos.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://anr.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://uxz.0kj1m.cn

JS:   arr.join(", ")
来源：http://dzh.ydzc1.top

TS:   arr.join(", ")
来源：http://ibf.meibo888.top

Java: String.join(", ", list)
来源：http://iro.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://ndk.fengsongda.top

Ruby: arr.join(", ")
来源：http://zkj.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://hex.zhoulong.xyz

================================================================================
来源：http://psd.sufxvd.cn

E. 字符串处理
来源：http://kko.chenjidiqi.icu

================================================================================
来源：http://wca.yueranfly.top

[E01] 拼接字符串
来源：http://jkb.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwi.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oep.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fip.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydd.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dqs.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yof.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xof.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kum.xuanzx.com

[E02] 重复字符串
来源：http://iwv.mhx1999.top

Py:   "ab" * 3
来源：http://pkv.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://ruc.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://sjw.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://mfg.yueranfly.top

Java: "ab".repeat(3)
来源：http://kku.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://jyh.ehwqpu.com

Ruby: "ab" * 3
来源：http://ayd.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qjk.yangfankeji.com

[E03] 截取子串
来源：http://pbd.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://naa.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://riz.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wyl.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://pco.yuxming.cn

Java: s.substring(1, 4)
来源：http://ask.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xbw.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yfh.meibo888.top

C#:   s.Substring(1, 3)
来源：http://eyr.bjfxy.top

[E04] 查找子串位置
来源：http://wzp.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://igb.sysykeji.top

PHP:  strpos($s, "x");
来源：http://iky.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tjj.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://xke.tian-w.cn

Java: s.indexOf("x")
来源：http://bbk.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://qce.xziqi.cn

Ruby: s.index("x")
来源：http://cxu.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://pbj.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kut.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bln.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://plb.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://odt.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hdq.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tom.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://izr.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vbz.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ibu.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://pxq.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fdz.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://dbe.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zrz.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://gqe.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://osk.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gsi.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gzn.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ymg.zdqjudy.top

[E07] 按分隔符拆分
来源：http://tvd.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://afe.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qfu.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://toe.sxryk.cn

TS:   s.split(",")
来源：http://opg.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://idr.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yzj.meibo888.top

Ruby: s.split(",");  s.split
来源：http://yav.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qzb.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://tvm.316326.xyz

Py:   ",".join(items)
来源：http://buw.yj20258888.top

PHP:  implode(",", $items);
来源：http://vli.yuxming.cn

JS:   items.join(",")
来源：http://nlx.cdnleiting.top

TS:   items.join(",")
来源：http://fze.hcnkem.com

Java: String.join(",", items)
来源：http://zbf.yj20258.top

Go:   strings.Join(items, ",")
来源：http://opl.gotoacloud.top

Ruby: items.join(",")
来源：http://cpu.guowangkeji.top

C#:   string.Join(",", items)
来源：http://tyu.hysaishi.cn

[E09] 去除所有空白字符
来源：http://krf.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cid.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ytj.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://rqo.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://ikk.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://ext.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xvr.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oey.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zhu.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://zpj.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yxa.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://svi.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://fva.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://aeo.tian-w.cn

Java: String.format("%03d", 7)
来源：http://uka.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uhz.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xbp.xuetiantiany.cn


<!-- 参考信息 -->