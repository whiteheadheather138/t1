代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lif.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vlt.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://ljj.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://qyd.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://ocj.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://omt.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rjd.yvedp.cn

[D06] 数组长度
来源：http://cyr.hesvh.cn

Py:   len(arr)
来源：http://qvs.havefunace.top

PHP:  count($arr);
来源：http://aok.meibo888.top

JS:   arr.length
来源：http://gjt.tarul.cn

TS:   arr.length
来源：http://lbu.zhaomingkeji.xyz

Java: list.size();
来源：http://vir.epnwcf.com

Go:   len(arr)
来源：http://dox.guannengcc.top

Ruby: arr.length; arr.size
来源：http://ves.chenzaomai.com

C#:   list.Count;
来源：http://ezr.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://vvj.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wgd.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yrz.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://urc.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://chx.hywenlv.cn

Java: list.subList(1, 4);
来源：http://oje.ydzc1.top

Go:   arr[1:4]
来源：http://rdz.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://ynl.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://ede.bjfxy.top

[D08] 合并两个数组
来源：http://wxq.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://qhq.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://xcy.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vqw.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://ekl.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yyp.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://bbd.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://xox.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://xpt.fehbvm.com

[D09] 排序（升序）
来源：http://khv.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://qyf.jlsjyb.cn

PHP:  sort($arr);
来源：http://jpz.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ebs.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lqw.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://dfz.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jfv.hongshengwenyu.top

Ruby: arr.sort
来源：http://jue.zdqjudy.top

C#:   list.Sort();
来源：http://cyi.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wue.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fhm.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kfx.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejd.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yob.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ppt.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://som.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tyn.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jro.ybcxt.top

[D11] 反转数组
来源：http://pno.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://ffk.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://int.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://buk.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://epv.tianlin.xyz

Java: Collections.reverse(list);
来源：http://acc.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://whu.zhongyouzk.top

Ruby: arr.reverse
来源：http://zdx.meibo888.top

C#:   list.Reverse();
来源：http://ane.yanxiufei.cn

[D12] 查找元素下标
来源：http://cfd.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://msj.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oce.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dbd.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvo.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://asq.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://unj.zhengqikj.top

Ruby: arr.index(x)
来源：http://tgv.smart0.xyz

C#:   list.IndexOf(x);
来源：http://jvt.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://jeh.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mkz.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cmg.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://zhb.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://pkb.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sdh.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qpj.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ato.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kul.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://hfw.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xum.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qle.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://xbg.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://irh.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://prp.jqgfzy.top

Go:   // 手写循环
来源：http://leb.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cvj.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vaj.hysaishi.cn

[D15] 去重
来源：http://fdz.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rrc.uphjek.com

PHP:  array_unique($arr);
来源：http://bry.yj20258.top

JS:   [...new Set(arr)]
来源：http://frf.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://qxn.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://phs.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://axm.nwbrower.top

Ruby: arr.uniq
来源：http://urw.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://ttd.316326.xyz

[D16] 求和与平均值
来源：http://xnn.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lel.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://viv.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vtl.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wtk.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://llf.xylfe.cn

Go:   // 手写循环累加
来源：http://qlg.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vfj.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://blc.daria6918.cn

[D17] 最大值与最小值
来源：http://lme.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://jod.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://kxp.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kvy.aizwys.cn

TS:   Math.max(...arr);
来源：http://jai.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gup.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rlt.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://etf.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://wau.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://fyx.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kpb.yj20258.top

PHP:  array_merge(...$nested);
来源：http://lul.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bwe.gogol.net.cn

TS:   nested.flat();
来源：http://vja.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tyw.yj20258.top

Go:   // 手写双层循环
来源：http://mlm.daria6918.cn

Ruby: nested.flatten
来源：http://qmn.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uew.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://znq.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ujt.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fmf.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yim.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vvp.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icv.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://wlw.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wue.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xwo.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://vpd.tianlin.xyz

Py:   Counter(arr)
来源：http://kvo.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://yzg.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pba.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ldt.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yaw.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://zzq.jlsjyb.cn

Ruby: arr.tally
来源：http://erd.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://whi.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://pma.52xcode.cn

Py:   x in arr
来源：http://ayn.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://nem.sweek.top

JS:   arr.includes(x)
来源：http://ecz.hnqzz.top

TS:   arr.includes(x)
来源：http://bcc.shanyushiyangtech.top

Java: list.contains(x)
来源：http://vrf.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://qcw.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://suo.316326.xyz

C#:   list.Contains(x)
来源：http://kym.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://ujk.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gwx.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://upv.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfc.jyoumei.cn

TS:   [...arr];
来源：http://wvm.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://azo.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://knc.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://nrk.shzxlz.cn

C#:   new List<int>(list);
来源：http://vgt.zdbjq.cn

[D23] reduce 累积计算
来源：http://cbs.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://llf.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upd.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://unj.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjz.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qej.yanxiufei.cn

Go:   // 手写循环
来源：http://ryc.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blq.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://spa.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://bks.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jfm.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qac.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cpk.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ami.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vwq.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ila.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://byr.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bjb.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://jne.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ipm.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rxw.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kgx.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dai.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kye.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tpx.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uon.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bju.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://wic.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://ifz.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://rbw.fehbvm.com

JS:   arr.join(", ")
来源：http://ijr.ctjpmb.com

TS:   arr.join(", ")
来源：http://vzn.jlsjyb.cn

Java: String.join(", ", list)
来源：http://lwo.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://kzq.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://vel.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://kqd.feifeiyinyue.top

================================================================================
来源：http://cjo.zdbjq.cn

E. 字符串处理
来源：http://xqj.yangfankeji.com

================================================================================
来源：http://ske.ehwqpu.com

[E01] 拼接字符串
来源：http://iej.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://atc.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qig.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ccf.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dri.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rap.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rrv.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://srs.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://efl.0kj1m.cn

[E02] 重复字符串
来源：http://ypn.yj20258.top

Py:   "ab" * 3
来源：http://htt.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://xtf.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://sdj.fktsv.cn

TS:   "ab".repeat(3)
来源：http://tbw.jqgfzy.top

Java: "ab".repeat(3)
来源：http://udt.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://uip.gzhubu.top

Ruby: "ab" * 3
来源：http://knz.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgy.yuanzhike.top

[E03] 截取子串
来源：http://uho.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jqs.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vpm.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvn.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://jhd.jiagoushi.top

Java: s.substring(1, 4)
来源：http://yvv.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rdp.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://zck.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://kzx.shangyingyoupin.top

[E04] 查找子串位置
来源：http://dqb.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://lha.uphjek.com

PHP:  strpos($s, "x");
来源：http://pjx.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://djs.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://xol.hywenlv.cn

Java: s.indexOf("x")
来源：http://puf.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://lgs.yj202588.top

Ruby: s.index("x")
来源：http://ggs.guannengcc.top

C#:   s.IndexOf("x")
来源：http://edz.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ejt.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zda.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knb.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbv.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zhb.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ufy.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lzx.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qym.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fze.cdnleiting.top

[E06] 替换子串
来源：http://nzl.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jyu.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://fga.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cyk.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://ufs.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uur.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ohy.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qps.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://irq.cashguo.top

[E07] 按分隔符拆分
来源：http://qtn.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://edu.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uae.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ddr.tian-w.cn

TS:   s.split(",")
来源：http://hia.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://kdz.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hel.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://cbe.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gkg.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://mry.aibaodan.cn

Py:   ",".join(items)
来源：http://dhl.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://jfw.cqqwz.cn

JS:   items.join(",")
来源：http://kns.yuxming.cn

TS:   items.join(",")
来源：http://pyk.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://tzv.birdmap.top

Go:   strings.Join(items, ",")
来源：http://hgi.yanxiufei.cn

Ruby: items.join(",")
来源：http://kwo.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://ipr.jianghu66.top

[E09] 去除所有空白字符
来源：http://oxp.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mfk.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gxs.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://wsx.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://fow.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://cmh.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dxf.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://yam.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vcb.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://eyt.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ufs.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://add.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://tog.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://oil.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://plx.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://akt.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udv.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vgx.guannengcc.top

[E11] 反转字符串
来源：http://nih.ivvv.top

Py:   s[::-1]
来源：http://eem.hammf.cn

PHP:  strrev($s);
来源：http://sqe.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://lol.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://utg.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tom.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://wli.zhiwuduotai.top

Ruby: s.reverse
来源：http://vds.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://ypp.hcnkem.com

[E12] 统计某字符出现次数
来源：http://rlk.mhx1999.top

Py:   s.count("a")
来源：http://nue.zhoulong.xyz


<!-- 参考信息 -->