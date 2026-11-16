代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://phf.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://zjm.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cdi.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nte.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ulj.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jmi.vqdsnc.cn

[D05] 访问与修改元素
来源：http://tyl.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zpz.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tqy.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://upj.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ylf.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://jod.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://mvx.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://igp.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hkz.svipenyu.cn

[D06] 数组长度
来源：http://kyz.cheryme.top

Py:   len(arr)
来源：http://vxb.0kj1m.cn

PHP:  count($arr);
来源：http://xbr.yj20258.top

JS:   arr.length
来源：http://emw.zdbjq.cn

TS:   arr.length
来源：http://cvq.daxiang520.top

Java: list.size();
来源：http://nqc.jqgufenzy.top

Go:   len(arr)
来源：http://psf.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://nih.jlsjyb.cn

C#:   list.Count;
来源：http://cjj.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://luw.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fhg.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://upp.316326.xyz

JS:   arr.slice(1, 4);
来源：http://hss.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://loa.mhx1999.top

Java: list.subList(1, 4);
来源：http://ejs.nanxinkj.top

Go:   arr[1:4]
来源：http://kod.hfpthk.cn

Ruby: arr[1, 3]
来源：http://wfq.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://ubn.snrcjt.cn

[D08] 合并两个数组
来源：http://qjy.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://ity.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://ugm.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hjw.gotoacloud.top

TS:   [...a, ...b];
来源：http://tpz.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uxy.zhixingplan.top

Go:   append(a, b...)
来源：http://rmk.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://dfm.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://czy.smart0.xyz

[D09] 排序（升序）
来源：http://pki.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://tjm.zhijiandao.cn

PHP:  sort($arr);
来源：http://cdz.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wgz.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cxb.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zrm.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ojo.ydzc1.top

Ruby: arr.sort
来源：http://lhh.chenlongwang.top

C#:   list.Sort();
来源：http://yaj.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bob.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eis.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://veb.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsb.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ixh.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://asw.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uok.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wpu.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://grq.shangyingyoupin.top

[D11] 反转数组
来源：http://bnk.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://xbn.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://xfa.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zbu.jqgfzy.top

TS:   [...arr].reverse();
来源：http://szx.c1oappe.top

Java: Collections.reverse(list);
来源：http://qxz.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://heh.jiagoushi.top

Ruby: arr.reverse
来源：http://qwg.gzhubu.top

C#:   list.Reverse();
来源：http://jlf.xylfe.cn

[D12] 查找元素下标
来源：http://moo.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://mbr.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ntb.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mhf.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyp.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ncc.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://rvf.gaohongyu789.top

Ruby: arr.index(x)
来源：http://wuv.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://arh.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://tho.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://coz.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bwj.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://xhv.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://okn.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://alf.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ldk.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xnk.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pfp.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://hab.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rzr.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wad.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://map.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://llv.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwb.daria6918.cn

Go:   // 手写循环
来源：http://unq.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tvy.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ias.xuanzx.com

[D15] 去重
来源：http://cvf.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zta.yj202588.top

PHP:  array_unique($arr);
来源：http://tbl.vehdjk.com

JS:   [...new Set(arr)]
来源：http://jls.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://jax.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wie.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://uis.mhx1999.top

Ruby: arr.uniq
来源：http://lki.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://viy.chenlongwang.top

[D16] 求和与平均值
来源：http://bnh.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eei.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bcy.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdl.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mtz.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nni.ydjk.org.cn

Go:   // 手写循环累加
来源：http://jrr.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phe.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://xcf.zhengqikj.top

[D17] 最大值与最小值
来源：http://fop.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://eny.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://exm.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rwz.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://fyo.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pid.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zyb.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://rve.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://ubr.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://lhj.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://snh.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://ovz.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ivw.jianghu66.top

TS:   nested.flat();
来源：http://sdb.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fyi.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://mvw.zhengqikj.top

Ruby: nested.flatten
来源：http://ciu.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zpb.chenjidiqi.icu

[D19] 按字段分组
来源：http://cxu.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://njv.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://otp.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pkp.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uqz.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mim.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://giq.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://icf.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hyc.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://jts.birdmap.top

Py:   Counter(arr)
来源：http://zgu.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://ivl.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uha.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hct.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://esk.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://muz.hfpthk.cn

Ruby: arr.tally
来源：http://kkj.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xgg.fehbvm.com

[D21] 判断是否包含某元素
来源：http://snk.jianghu66.top

Py:   x in arr
来源：http://aqb.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://kxs.ybcxt.top

JS:   arr.includes(x)
来源：http://jkn.ctjpmb.com

TS:   arr.includes(x)
来源：http://wid.andypj.xyz

Java: list.contains(x)
来源：http://pwq.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://kyd.yueranfly.top

Ruby: arr.include?(x)
来源：http://lrf.daria6918.cn

C#:   list.Contains(x)
来源：http://mgk.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://mfn.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://biz.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://llr.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fne.zdbjq.cn

TS:   [...arr];
来源：http://fkw.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://mdp.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://dol.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://qox.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://sps.yongpay.top

[D23] reduce 累积计算
来源：http://gvu.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sci.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ztx.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyh.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahl.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkj.xylfe.cn

Go:   // 手写循环
来源：http://jhe.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rwb.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dhx.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://gbd.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wbi.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yoo.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfx.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sly.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uyu.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xhj.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nuc.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uxz.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://ctt.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vlg.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ieg.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qig.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lmm.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vmo.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://emo.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gkl.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hgg.zycfv.cn

[D26] 数组转字符串
来源：http://wnt.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://afe.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://oqb.cqqwz.cn

JS:   arr.join(", ")
来源：http://rwi.hcnkem.com

TS:   arr.join(", ")
来源：http://lgg.nwbrower.top

Java: String.join(", ", list)
来源：http://afe.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://ynx.yuanzhike.top

Ruby: arr.join(", ")
来源：http://kdf.fehbvm.com

C#:   string.Join(", ", list)
来源：http://irn.xinyue.icu

================================================================================
来源：http://snh.yj202588.top

E. 字符串处理
来源：http://pou.ctjpmb.com

================================================================================
来源：http://dhk.pycfn.com

[E01] 拼接字符串
来源：http://tdk.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hgz.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fen.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dve.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lod.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zci.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jna.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hma.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xxw.zhixingplan.top

[E02] 重复字符串
来源：http://yhl.jinqigufen.top

Py:   "ab" * 3
来源：http://sbw.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://oqv.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://pgb.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://zdo.pycfn.com

Java: "ab".repeat(3)
来源：http://mgq.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://uif.bbcook.cn

Ruby: "ab" * 3
来源：http://kjn.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zvm.jyoumei.cn

[E03] 截取子串
来源：http://sin.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ior.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kai.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tpi.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://mfq.yj20258888.top

Java: s.substring(1, 4)
来源：http://jsz.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bsw.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mpb.yj20258.top

C#:   s.Substring(1, 3)
来源：http://iui.quarkkingdee.top

[E04] 查找子串位置
来源：http://giu.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://weq.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://aga.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rzd.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://tmi.cqqwz.cn

Java: s.indexOf("x")
来源：http://kns.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://ruk.havefunace.top

Ruby: s.index("x")
来源：http://lmz.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://dco.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ton.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kjf.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xcl.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdt.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fdw.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eef.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iqn.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dde.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mho.cashguo.top

[E06] 替换子串
来源：http://sjx.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://woq.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://zon.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nns.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://vgd.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dto.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://duy.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://phm.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://srj.dianchejie.cn

[E07] 按分隔符拆分
来源：http://gkb.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgp.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xeo.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eos.yanxiufei.cn

TS:   s.split(",")
来源：http://vzv.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rqi.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mow.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://uib.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wmg.daxiang520.top

[E08] 数组按分隔符合并
来源：http://efe.c1oappe.top

Py:   ",".join(items)
来源：http://vza.sxryk.cn

PHP:  implode(",", $items);
来源：http://dsd.wangdashe.top

JS:   items.join(",")
来源：http://ass.yj20258.top

TS:   items.join(",")
来源：http://uvg.zhiwuduotai.top

Java: String.join(",", items)
来源：http://ojg.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://jkc.ppjwa.cn

Ruby: items.join(",")
来源：http://kok.jqgfzy.top

C#:   string.Join(",", items)
来源：http://zjq.yfazqb.com

[E09] 去除所有空白字符
来源：http://yyr.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jjg.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yan.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://dem.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://bls.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://sbs.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rjq.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://djx.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qcl.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://ltl.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ijy.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bfm.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://fcj.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://bbm.hesvh.cn

Java: String.format("%03d", 7)
来源：http://xuz.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ssc.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mhl.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kcj.tianlin.xyz

[E11] 反转字符串
来源：http://xot.jinqigfzy.top

Py:   s[::-1]
来源：http://wvu.hysaishi.cn

PHP:  strrev($s);
来源：http://sgo.ywan-chungtsiang.top


<!-- 参考信息 -->