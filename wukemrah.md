代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://dlg.pycfn.com

Java: list.add(0, 0);
来源：http://vaa.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sii.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tjf.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://tpq.shangyingyoupin.top

[D04] 删除元素
来源：http://wvq.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jgk.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bgs.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ccm.pycfn.com

TS:   arr.splice(0, 1);
来源：http://pte.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://irb.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aie.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wwj.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mmu.yuanzhike.top

[D05] 访问与修改元素
来源：http://fzl.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxt.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xuy.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eoo.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://qco.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://nsm.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://osi.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ixw.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vei.yvedp.cn

[D06] 数组长度
来源：http://oqz.vehdjk.com

Py:   len(arr)
来源：http://iyz.hammf.cn

PHP:  count($arr);
来源：http://kpm.shuidangran.top

JS:   arr.length
来源：http://hgu.bbcook.cn

TS:   arr.length
来源：http://ysl.sjlbkw.cn

Java: list.size();
来源：http://znp.zycfv.cn

Go:   len(arr)
来源：http://cwc.xinyue.icu

Ruby: arr.length; arr.size
来源：http://viv.ydjk.org.cn

C#:   list.Count;
来源：http://aek.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://uuh.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://egg.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://wwy.316326.xyz

JS:   arr.slice(1, 4);
来源：http://yha.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://jun.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://qop.iojbl.cn

Go:   arr[1:4]
来源：http://wvi.ivvv.top

Ruby: arr[1, 3]
来源：http://tvp.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://dzq.hcnkem.com

[D08] 合并两个数组
来源：http://ofh.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://xtl.yj20258.top

PHP:  array_merge($a, $b);
来源：http://ptw.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cnv.316326.xyz

TS:   [...a, ...b];
来源：http://auq.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lur.sufxvd.cn

Go:   append(a, b...)
来源：http://nah.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://avj.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://elx.jianghu66.top

[D09] 排序（升序）
来源：http://mfr.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://bfn.zhoulong.xyz

PHP:  sort($arr);
来源：http://btg.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wfs.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pvg.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lhc.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bkd.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://rxa.yvedp.cn

C#:   list.Sort();
来源：http://ypt.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jyp.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nno.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gpp.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://agg.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfe.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zzg.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zmg.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ros.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ifw.shanyushiyangkeji.top

[D11] 反转数组
来源：http://gny.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lbh.guannengcc.top

PHP:  array_reverse($arr);
来源：http://vki.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dff.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://aul.yangfankeji.com

Java: Collections.reverse(list);
来源：http://uod.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://hbu.redwolf501.top

Ruby: arr.reverse
来源：http://bqr.zycfv.cn

C#:   list.Reverse();
来源：http://olv.chenlongwang.top

[D12] 查找元素下标
来源：http://llx.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://iix.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbk.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://idm.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gjt.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iol.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://svf.yueranfly.top

Ruby: arr.index(x)
来源：http://qzs.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://kzx.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://bpf.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pcn.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://edz.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://biu.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://mjs.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tur.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fic.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://ymq.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dtw.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://qev.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lpd.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cca.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://shz.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://cvg.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://lvj.zycfv.cn

Go:   // 手写循环
来源：http://iui.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://tdm.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://igk.zdbjq.cn

[D15] 去重
来源：http://epi.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rmb.52xcode.cn

PHP:  array_unique($arr);
来源：http://hir.cheryme.top

JS:   [...new Set(arr)]
来源：http://zat.316326.xyz

TS:   [...new Set(arr)]
来源：http://thv.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ihc.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://agy.guowangkeji.top

Ruby: arr.uniq
来源：http://iko.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://oqu.yj202588.top

[D16] 求和与平均值
来源：http://ehi.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ldw.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hlv.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkl.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://duh.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://knx.yj202588.top

Go:   // 手写循环累加
来源：http://xtq.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jbv.sweek.top

C#:   list.Sum();  list.Average()
来源：http://xny.zdqjudy.top

[D17] 最大值与最小值
来源：http://smr.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://eqy.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://nhl.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vwf.yongpay.top

TS:   Math.max(...arr);
来源：http://jbw.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://afz.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ljo.uphjek.com

Ruby: arr.max;  arr.min
来源：http://jlq.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://snt.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://raj.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wpu.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://nka.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yvn.wangshuangyany.cn

TS:   nested.flat();
来源：http://vey.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://csc.kuanghao11.cn

Go:   // 手写双层循环
来源：http://eaw.tarul.cn

Ruby: nested.flatten
来源：http://smt.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://elh.gotoacloud.top

[D19] 按字段分组
来源：http://ldh.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gwe.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvy.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nog.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rqg.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tmg.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://odg.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dru.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jgt.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://zkk.quarkkingdee.top

Py:   Counter(arr)
来源：http://whb.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://fvb.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwb.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kjp.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vlv.cheryme.top

Go:   // 手写 map[T]int
来源：http://itl.hnqzz.top

Ruby: arr.tally
来源：http://tqf.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://osv.zycfv.cn

[D21] 判断是否包含某元素
来源：http://tup.epnwcf.com

Py:   x in arr
来源：http://ulb.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://szc.ctjpmb.com

JS:   arr.includes(x)
来源：http://xbb.aizwys.cn

TS:   arr.includes(x)
来源：http://fqv.svipenyu.cn

Java: list.contains(x)
来源：http://hdr.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://xny.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://bsr.zhoulong.xyz

C#:   list.Contains(x)
来源：http://aas.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://aaz.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pxv.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xtx.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mre.yuanzhike.top

TS:   [...arr];
来源：http://cee.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://kwz.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://ybo.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://mis.jlsjyb.cn

C#:   new List<int>(list);
来源：http://bfe.gotoacloud.top

[D23] reduce 累积计算
来源：http://kzq.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fmf.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kaw.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ske.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lgl.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nom.gaohongyu789.top

Go:   // 手写循环
来源：http://nid.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyx.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bri.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://tdf.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vpz.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ije.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rwr.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cvw.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eho.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kcm.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jrt.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://edc.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://tjg.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jmk.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bhp.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nws.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sce.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mms.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qlw.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qvz.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sqe.nwbrower.top

[D26] 数组转字符串
来源：http://mnk.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://nma.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://pqe.zhixingplan.top

JS:   arr.join(", ")
来源：http://akn.yangfankeji.com

TS:   arr.join(", ")
来源：http://arb.fengsongda.top

Java: String.join(", ", list)
来源：http://kbv.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://sjo.gzhubu.top

Ruby: arr.join(", ")
来源：http://wpc.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://coh.fengsongda.top

================================================================================
来源：http://qsh.uphjek.com

E. 字符串处理
来源：http://rtm.nwbrower.top

================================================================================
来源：http://xkd.meibo888.top

[E01] 拼接字符串
来源：http://pgs.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vzx.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://csj.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://usn.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iru.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ukh.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://svg.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uwq.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://noq.nanxuanxn.top

[E02] 重复字符串
来源：http://jnu.chenlongwang.top

Py:   "ab" * 3
来源：http://gam.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://lot.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://jjc.316326.xyz

TS:   "ab".repeat(3)
来源：http://gon.bjfxy.top

Java: "ab".repeat(3)
来源：http://qbk.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://aec.hysaishi.cn

Ruby: "ab" * 3
来源：http://tgu.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://anu.yueranfly.top

[E03] 截取子串
来源：http://uin.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ivy.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://npj.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://khz.daxiang520.top

TS:   s.slice(1, 4)
来源：http://boz.9152youxi.cn

Java: s.substring(1, 4)
来源：http://wpf.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rnm.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://ssn.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://ukt.daria6918.cn

[E04] 查找子串位置
来源：http://ebk.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://ovk.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://ipn.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zud.fengsongda.top

TS:   s.indexOf("x")
来源：http://rju.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://cbb.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://ols.zdbjq.cn

Ruby: s.index("x")
来源：http://cqm.aizwys.cn

C#:   s.IndexOf("x")
来源：http://yuh.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuw.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ajt.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lix.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://opc.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://mzi.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dju.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezq.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nav.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oev.yuxming.cn

[E06] 替换子串
来源：http://qgu.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rfa.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://sbj.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zuv.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://yfr.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wlx.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fod.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qqo.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://gnn.zdbjq.cn

[E07] 按分隔符拆分
来源：http://igx.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ckx.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://djf.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tmp.birdmap.top

TS:   s.split(",")
来源：http://fpq.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nnb.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dor.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://aqj.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://niz.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://ypu.zhixingplan.top

Py:   ",".join(items)
来源：http://tna.yuxming.cn

PHP:  implode(",", $items);
来源：http://svn.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://yiz.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://npx.52xcode.cn

Java: String.join(",", items)
来源：http://qzd.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://tvt.hammf.cn

Ruby: items.join(",")
来源：http://wxb.ybcxt.top

C#:   string.Join(",", items)
来源：http://whr.yongpay.top

[E09] 去除所有空白字符
来源：http://fkz.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://obf.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zkv.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://iyx.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://gtm.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://gnc.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pka.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://jdm.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ozr.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://fyl.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nfl.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cwt.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://hgj.sweek.top


<!-- 参考信息 -->