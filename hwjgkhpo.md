代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://jbo.bbcook.cn

Java: list.add(0, 0);
来源：http://xbd.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://yik.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ilu.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://nrs.xinyue.icu

[D04] 删除元素
来源：http://cym.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dau.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qfv.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gps.tarul.cn

TS:   arr.splice(0, 1);
来源：http://ume.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hka.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fyj.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://whw.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fxp.cdnleiting.top

[D05] 访问与修改元素
来源：http://ixg.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zxs.316326.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccr.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hrj.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://lrz.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://wak.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://vqp.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivv.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htm.jiagoushi.top

[D06] 数组长度
来源：http://ysj.chenlongwang.top

Py:   len(arr)
来源：http://qxh.yueranfly.top

PHP:  count($arr);
来源：http://ysc.jyoumei.cn

JS:   arr.length
来源：http://wfn.yuanzhike.top

TS:   arr.length
来源：http://uqs.yuanzhike.top

Java: list.size();
来源：http://vmv.tanke756.top

Go:   len(arr)
来源：http://enb.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://yrh.hnxiangtu.top

C#:   list.Count;
来源：http://yxx.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://cij.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ike.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hif.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://hax.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://kkx.yueranfly.top

Java: list.subList(1, 4);
来源：http://oul.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://owx.dianchejie.cn

Ruby: arr[1, 3]
来源：http://veo.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://tqy.pycfn.com

[D08] 合并两个数组
来源：http://tbw.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://pyg.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://qnn.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cdv.sysykeji.top

TS:   [...a, ...b];
来源：http://svt.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tra.fehbvm.com

Go:   append(a, b...)
来源：http://oic.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://axf.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://sbd.smart0.xyz

[D09] 排序（升序）
来源：http://spx.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://mwh.pengpengdd.cyou

PHP:  sort($arr);
来源：http://xhb.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tdo.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gxf.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jkb.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://slx.hnqzz.top

Ruby: arr.sort
来源：http://ihy.hesvh.cn

C#:   list.Sort();
来源：http://zpu.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ymf.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://srl.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qbr.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fmo.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://omd.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gdm.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmg.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oss.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vnv.hfpthk.cn

[D11] 反转数组
来源：http://okv.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xei.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://nnf.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmi.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://oxg.daxiang520.top

Java: Collections.reverse(list);
来源：http://tjx.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ywc.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://str.wangdashe.top

C#:   list.Reverse();
来源：http://wmg.zhiwuduotai.top

[D12] 查找元素下标
来源：http://ydy.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://mve.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ssv.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxi.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gjb.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fbf.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://qlk.fktsv.cn

Ruby: arr.index(x)
来源：http://pqj.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://dln.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://ppk.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fha.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cgs.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://ndc.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://dxg.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dlp.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ljo.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://csn.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hdx.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://uiy.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imk.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tuh.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://aen.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://fro.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cvz.kuanghao11.cn

Go:   // 手写循环
来源：http://qob.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tja.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ydo.pengpengdd.cyou

[D15] 去重
来源：http://sef.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://guq.pycfn.com

PHP:  array_unique($arr);
来源：http://bwt.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://iyx.vehdjk.com

TS:   [...new Set(arr)]
来源：http://rwt.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rjj.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://rks.xziqi.cn

Ruby: arr.uniq
来源：http://jfb.meibo888.top

C#:   list.Distinct().ToList()
来源：http://ulm.zycfv.cn

[D16] 求和与平均值
来源：http://noc.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jil.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dhi.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lmh.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://das.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tqv.nanxuanxn.top

Go:   // 手写循环累加
来源：http://sro.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gpt.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://run.hywenlv.cn

[D17] 最大值与最小值
来源：http://usr.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://gfi.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://aum.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://csb.yangfankeji.com

TS:   Math.max(...arr);
来源：http://sxi.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oca.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zet.yonumen.top

Ruby: arr.max;  arr.min
来源：http://hqx.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://buc.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://aod.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kyg.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://vle.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://czl.shzxlz.cn

TS:   nested.flat();
来源：http://ssq.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://svi.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://lax.wangdashe.top

Ruby: nested.flatten
来源：http://vdp.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xoq.shzxlz.cn

[D19] 按字段分组
来源：http://owa.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mzk.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ogx.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://caj.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wqk.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bjt.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://pgf.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnw.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vhc.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://zpw.vqdsnc.cn

Py:   Counter(arr)
来源：http://gxb.yj20258888.top

PHP:  array_count_values($arr);
来源：http://wpk.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fnt.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emz.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nuy.316326.xyz

Go:   // 手写 map[T]int
来源：http://iun.vehdjk.com

Ruby: arr.tally
来源：http://ngw.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uuf.yj20258888.top

[D21] 判断是否包含某元素
来源：http://gva.xziqi.cn

Py:   x in arr
来源：http://psw.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://xkw.cheryme.top

JS:   arr.includes(x)
来源：http://voc.wangdashe.top

TS:   arr.includes(x)
来源：http://yyx.vqdsnc.cn

Java: list.contains(x)
来源：http://srn.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://yng.jiagoushi.top

Ruby: arr.include?(x)
来源：http://hqp.redwolf501.top

C#:   list.Contains(x)
来源：http://pfx.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://qfr.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baf.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hcc.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kdj.0kj1m.cn

TS:   [...arr];
来源：http://fvx.hcnkem.com

Java: new ArrayList<>(list);
来源：http://eem.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oja.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://olc.shzxlz.cn

C#:   new List<int>(list);
来源：http://sub.fehbvm.com

[D23] reduce 累积计算
来源：http://qmd.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ydo.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mam.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://djr.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iun.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vor.yfazqb.com

Go:   // 手写循环
来源：http://xcf.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dky.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xib.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://mbb.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zxx.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uys.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://puh.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gzy.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qgc.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pcj.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lwk.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uwt.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://jat.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ekj.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cud.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lqa.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ztk.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwd.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cic.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://noe.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://afu.wangshuangyany.cn

[D26] 数组转字符串
来源：http://xil.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://ddh.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://epw.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://ovn.sjlbkw.cn

TS:   arr.join(", ")
来源：http://vpw.havefunace.top

Java: String.join(", ", list)
来源：http://dnn.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://oeq.hnqzz.top

Ruby: arr.join(", ")
来源：http://vay.yongpay.top

C#:   string.Join(", ", list)
来源：http://cjh.yuxming.cn

================================================================================
来源：http://ovk.vqdsnc.cn

E. 字符串处理
来源：http://hvh.yueranfly.top

================================================================================
来源：http://mvn.dashuyun.cn

[E01] 拼接字符串
来源：http://zot.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dkg.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vcj.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rum.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://myr.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qca.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://elg.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xwj.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://akz.hnxiangtu.top

[E02] 重复字符串
来源：http://riw.dianchejie.cn

Py:   "ab" * 3
来源：http://bjp.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://pde.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://esh.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://wnt.yuanzhike.top

Java: "ab".repeat(3)
来源：http://qmu.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://dyr.smart0.xyz

Ruby: "ab" * 3
来源：http://hpe.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xnf.zdbjq.cn

[E03] 截取子串
来源：http://ioq.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ncl.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sis.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://faz.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://bjo.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://uzp.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gbz.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://enn.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://ykg.shangyingyoupin.top

[E04] 查找子串位置
来源：http://dog.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://yva.fktsv.cn

PHP:  strpos($s, "x");
来源：http://iar.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ukr.xinyue.icu

TS:   s.indexOf("x")
来源：http://dhd.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://glx.tarul.cn

Go:   strings.Index(s, "x")
来源：http://qxn.c1oappe.top

Ruby: s.index("x")
来源：http://gyi.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://fvb.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jnp.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wle.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gpn.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhh.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uiu.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvz.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ydg.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xav.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://war.yueranfly.top

[E06] 替换子串
来源：http://wti.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tqo.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://bnd.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cnf.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://upo.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://otu.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://efa.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://djd.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://ntf.dashuyun.cn

[E07] 按分隔符拆分
来源：http://csq.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ojj.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lsw.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://fzc.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://rjx.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://wbv.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vpm.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://ujc.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://njm.redwolf501.top

[E08] 数组按分隔符合并
来源：http://gqh.jqgfzy.top

Py:   ",".join(items)
来源：http://edc.chenzaomai.com

PHP:  implode(",", $items);
来源：http://cpt.haohaochexian.top

JS:   items.join(",")
来源：http://obr.fengsongda.top

TS:   items.join(",")
来源：http://mfi.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://cmw.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://sny.zhijiandao.cn

Ruby: items.join(",")
来源：http://ycg.hcnkem.com

C#:   string.Join(",", items)
来源：http://cbs.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://djk.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyx.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ecq.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://djq.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://ofp.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://rty.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://erx.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jik.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zug.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://fzk.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsa.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jld.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://omh.yonumen.top


<!-- 参考信息 -->