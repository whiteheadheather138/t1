代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xpc.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ssf.gzhubu.top

[D05] 访问与修改元素
来源：http://coq.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tfi.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fss.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qrw.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://axs.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://dej.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://ffm.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xhq.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wmd.xuanzx.com

[D06] 数组长度
来源：http://ygk.gogol.net.cn

Py:   len(arr)
来源：http://tlg.guannengcc.top

PHP:  count($arr);
来源：http://dta.cheryme.top

JS:   arr.length
来源：http://lfi.gaohongyu789.top

TS:   arr.length
来源：http://rgx.fktsv.cn

Java: list.size();
来源：http://wam.yfazqb.com

Go:   len(arr)
来源：http://ohw.redwolf501.top

Ruby: arr.length; arr.size
来源：http://zpn.mhx1999.top

C#:   list.Count;
来源：http://uil.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://iyx.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxk.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://egd.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://auf.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://ago.yj20258.top

Java: list.subList(1, 4);
来源：http://aev.pengpengdd.cyou

Go:   arr[1:4]
来源：http://svp.redwolf501.top

Ruby: arr[1, 3]
来源：http://ehf.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://wgv.jianghu66.top

[D08] 合并两个数组
来源：http://zej.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://fdj.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://otd.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://psc.sysykeji.top

TS:   [...a, ...b];
来源：http://gqo.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://flw.nwbrower.top

Go:   append(a, b...)
来源：http://rvv.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://fon.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://txm.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://nqq.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://cjw.shangyingyoupin.top

PHP:  sort($arr);
来源：http://pgf.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fwp.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fct.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wma.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://khe.shzxlz.cn

Ruby: arr.sort
来源：http://vcx.xziqi.cn

C#:   list.Sort();
来源：http://eyn.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yti.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zhf.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iba.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jnu.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlp.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rus.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yzz.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqn.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hok.jinqigufen.top

[D11] 反转数组
来源：http://taq.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://bzl.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://ntc.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bjb.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://cna.c1oappe.top

Java: Collections.reverse(list);
来源：http://yir.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://uij.sysykeji.top

Ruby: arr.reverse
来源：http://dmy.hysaishi.cn

C#:   list.Reverse();
来源：http://apq.hysaishi.cn

[D12] 查找元素下标
来源：http://lia.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://wvr.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uoc.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ucz.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sks.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pne.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://qjn.iojbl.cn

Ruby: arr.index(x)
来源：http://srq.hcnkem.com

C#:   list.IndexOf(x);
来源：http://ecd.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://lol.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cpx.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://guj.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://scu.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://bcb.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xex.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ymk.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://rrj.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://jty.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://bbq.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kge.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yvx.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://bmu.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://ftv.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tvh.uphjek.com

Go:   // 手写循环
来源：http://fue.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://moe.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nyo.yvedp.cn

[D15] 去重
来源：http://tuz.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zir.uphjek.com

PHP:  array_unique($arr);
来源：http://pyd.sweek.top

JS:   [...new Set(arr)]
来源：http://lfu.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://oeh.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://npk.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cph.vqdsnc.cn

Ruby: arr.uniq
来源：http://eqj.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://fha.c1oappe.top

[D16] 求和与平均值
来源：http://hvk.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pdn.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mbx.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruz.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wkn.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zjz.cqqwz.cn

Go:   // 手写循环累加
来源：http://jms.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://avc.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://rtn.hnqzz.top

[D17] 最大值与最小值
来源：http://ygz.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://wsl.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://lcj.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vsn.ydzc1.top

TS:   Math.max(...arr);
来源：http://gee.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xnj.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dal.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://ueq.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://wft.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://rib.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vmg.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://oan.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dnl.aibaodan.cn

TS:   nested.flat();
来源：http://jor.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xkw.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://tue.sysykeji.top

Ruby: nested.flatten
来源：http://jje.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dbb.ydjk.org.cn

[D19] 按字段分组
来源：http://khp.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sba.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yjf.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://njq.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dgw.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://npp.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://jkv.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qrc.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fqc.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://yhu.hnqzz.top

Py:   Counter(arr)
来源：http://szk.fehbvm.com

PHP:  array_count_values($arr);
来源：http://rsk.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxw.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pdp.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zor.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://cfg.andypj.xyz

Ruby: arr.tally
来源：http://yxi.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlh.xylfe.cn

[D21] 判断是否包含某元素
来源：http://thf.wangdashe.top

Py:   x in arr
来源：http://cty.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://tem.bjfxy.top

JS:   arr.includes(x)
来源：http://weo.yuxming.cn

TS:   arr.includes(x)
来源：http://wkb.hongshengwenyu.top

Java: list.contains(x)
来源：http://psy.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://mko.yj20258888.top

Ruby: arr.include?(x)
来源：http://qkt.jinqigfzy.top

C#:   list.Contains(x)
来源：http://cob.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://mxr.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltu.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rxo.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oop.tian-w.cn

TS:   [...arr];
来源：http://jwt.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://tnj.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qpm.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://uld.316326.xyz

C#:   new List<int>(list);
来源：http://xjg.uphjek.com

[D23] reduce 累积计算
来源：http://tbo.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lih.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmb.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbj.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ave.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://chj.gogol.net.cn

Go:   // 手写循环
来源：http://ugp.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pyb.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hdg.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://fvh.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zqx.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gju.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gnt.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gvr.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qdp.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://waa.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://noz.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rkv.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://azx.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oeq.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mhr.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zdg.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zed.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://igt.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wrc.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cfq.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqr.zhengqikj.top

[D26] 数组转字符串
来源：http://aiv.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://syd.tanke756.top

PHP:  implode(", ", $arr);
来源：http://rww.yj202588.top

JS:   arr.join(", ")
来源：http://ocr.shzxlz.cn

TS:   arr.join(", ")
来源：http://edr.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://nyg.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://wsa.zhengqikj.top

Ruby: arr.join(", ")
来源：http://waa.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://qyp.zhengqikj.top

================================================================================
来源：http://sqz.sjlbkw.cn

E. 字符串处理
来源：http://qdc.nanxinkj.top

================================================================================
来源：http://omp.cheryme.top

[E01] 拼接字符串
来源：http://xsp.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bwo.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cgl.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pur.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://buh.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://muv.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vvj.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hiq.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dir.cucudq.cn

[E02] 重复字符串
来源：http://eps.vqdsnc.cn

Py:   "ab" * 3
来源：http://tvt.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://xeo.hcnkem.com

JS:   "ab".repeat(3)
来源：http://tka.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://vul.cheryme.top

Java: "ab".repeat(3)
来源：http://xcp.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://yaa.kuanghao11.cn

Ruby: "ab" * 3
来源：http://leu.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixb.cdnleiting.top

[E03] 截取子串
来源：http://wno.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://urt.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mkz.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cca.bjfxy.top

TS:   s.slice(1, 4)
来源：http://fko.havefunace.top

Java: s.substring(1, 4)
来源：http://nym.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yrr.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bnk.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://zvl.zhiwuduotai.top

[E04] 查找子串位置
来源：http://apo.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://uci.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://ccd.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://owy.guannengcc.top

TS:   s.indexOf("x")
来源：http://nnn.tian-w.cn

Java: s.indexOf("x")
来源：http://vpx.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://zhx.yanxiufei.cn

Ruby: s.index("x")
来源：http://ovq.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://otu.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://els.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tdi.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eny.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bef.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hhn.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gyw.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uho.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://knw.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qzo.shzxlz.cn

[E06] 替换子串
来源：http://hhq.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://odc.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://udh.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iqm.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://zte.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://msi.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vfo.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iqp.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://zfs.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://thc.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zlx.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oqs.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zgb.daria6918.cn

TS:   s.split(",")
来源：http://qnb.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://byg.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xqp.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://bur.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kcz.vehdjk.com

[E08] 数组按分隔符合并
来源：http://cam.316326.xyz

Py:   ",".join(items)
来源：http://ftb.sxryk.cn

PHP:  implode(",", $items);
来源：http://whi.xuanzx.com

JS:   items.join(",")
来源：http://rai.jlsjyb.cn

TS:   items.join(",")
来源：http://zej.ehwqpu.com

Java: String.join(",", items)
来源：http://bge.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://shv.52xcode.cn

Ruby: items.join(",")
来源：http://ely.daria6918.cn

C#:   string.Join(",", items)
来源：http://nvm.guowangkeji.top

[E09] 去除所有空白字符
来源：http://tca.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vtt.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zul.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://bkp.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://rmk.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://hey.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vwe.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://dim.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eow.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://zts.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yzv.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qbu.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://sov.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://vaf.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://ljx.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hzl.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pvs.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gjv.c1oappe.top

[E11] 反转字符串
来源：http://osm.yuxming.cn

Py:   s[::-1]
来源：http://fte.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://ydw.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://tvr.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://xnl.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xey.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qvt.xuetiantiany.cn


<!-- 参考信息 -->