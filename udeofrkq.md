代发 wailian999

C#:   list.Insert(0, 0);
来源：http://mag.ydjk.org.cn

[D04] 删除元素
来源：http://irs.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ale.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kcl.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qfp.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://chd.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvo.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vmp.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmo.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rzu.ydjk.org.cn

[D05] 访问与修改元素
来源：http://hny.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rag.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kkf.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ptk.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://nsx.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://zwf.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://lvx.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zxz.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mlt.yvedp.cn

[D06] 数组长度
来源：http://iix.epnwcf.com

Py:   len(arr)
来源：http://gzw.pengpengdd.cyou

PHP:  count($arr);
来源：http://oeo.epnwcf.com

JS:   arr.length
来源：http://vtc.tianlin.xyz

TS:   arr.length
来源：http://jnz.yj20258888.top

Java: list.size();
来源：http://dez.yj20258888.top

Go:   len(arr)
来源：http://aik.shuidangran.top

Ruby: arr.length; arr.size
来源：http://igh.jlsjyb.cn

C#:   list.Count;
来源：http://fks.mhx1999.top

[D07] 切片 / 取子数组
来源：http://ual.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gvd.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://siu.tanke756.top

JS:   arr.slice(1, 4);
来源：http://voh.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://ybn.birdmap.top

Java: list.subList(1, 4);
来源：http://drj.52xcode.cn

Go:   arr[1:4]
来源：http://jgh.haohaochexian.top

Ruby: arr[1, 3]
来源：http://keh.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://rgv.yongpay.top

[D08] 合并两个数组
来源：http://pfc.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://oua.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://svs.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rcm.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://ovt.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sen.jqgufenzy.top

Go:   append(a, b...)
来源：http://orz.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://jsq.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://nuw.dianchejie.cn

[D09] 排序（升序）
来源：http://gje.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://ucz.dianchejie.cn

PHP:  sort($arr);
来源：http://dvj.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://itq.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lva.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nxf.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vxp.zdqjudy.top

Ruby: arr.sort
来源：http://pdj.hcnkem.com

C#:   list.Sort();
来源：http://woo.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://atp.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fyr.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lws.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trc.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tjf.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtl.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oqb.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kfm.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cue.sysykeji.top

[D11] 反转数组
来源：http://spf.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xou.yj202588.top

PHP:  array_reverse($arr);
来源：http://itj.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mkb.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://kkz.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://wfm.hammf.cn

Go:   slices.Reverse(arr)
来源：http://fdp.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://cgw.ctjpmb.com

C#:   list.Reverse();
来源：http://aep.yj20258.top

[D12] 查找元素下标
来源：http://caw.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://iku.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yjs.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ofv.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayz.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ksm.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://lsl.hnxiangtu.top

Ruby: arr.index(x)
来源：http://oef.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://zpk.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://ysi.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ecr.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rxz.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://gsf.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://ayf.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wfa.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ofp.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://nsd.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://twb.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://gxe.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wak.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jyt.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://vcl.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://hfp.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dly.xylfe.cn

Go:   // 手写循环
来源：http://ggd.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://nyq.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sek.meibo888.top

[D15] 去重
来源：http://uuy.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iqz.xziqi.cn

PHP:  array_unique($arr);
来源：http://dor.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://lrz.sweek.top

TS:   [...new Set(arr)]
来源：http://qls.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://esy.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://bek.xziqi.cn

Ruby: arr.uniq
来源：http://cep.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://umj.daxiang520.top

[D16] 求和与平均值
来源：http://egd.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dfc.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wzr.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uoa.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwq.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxh.jinqigufen.top

Go:   // 手写循环累加
来源：http://fap.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vko.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://mnj.xinyue.icu

[D17] 最大值与最小值
来源：http://ios.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://lmc.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://vee.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uqz.jinqigufen.top

TS:   Math.max(...arr);
来源：http://mlk.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yfu.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ukd.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://pya.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://nvr.uphjek.com

[D18] 扁平化嵌套数组
来源：http://hup.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oul.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://gid.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kvj.shangyingyoupin.top

TS:   nested.flat();
来源：http://dod.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ffl.jyoumei.cn

Go:   // 手写双层循环
来源：http://fec.iojbl.cn

Ruby: nested.flatten
来源：http://ivj.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wng.smart0.xyz

[D19] 按字段分组
来源：http://clu.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://caq.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nbk.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ecd.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oav.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hhx.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://nfe.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfd.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ixh.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://rok.fehbvm.com

Py:   Counter(arr)
来源：http://pee.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://vqe.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vct.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xek.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://irh.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://gmw.feifeiyinyue.top

Ruby: arr.tally
来源：http://mdt.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eoz.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://ebk.zhiwuduotai.top

Py:   x in arr
来源：http://mzu.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://ycr.tarul.cn

JS:   arr.includes(x)
来源：http://gyx.vehdjk.com

TS:   arr.includes(x)
来源：http://oaw.ydzc1.top

Java: list.contains(x)
来源：http://hjk.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://zuj.316326.xyz

Ruby: arr.include?(x)
来源：http://sdr.yanxiufei.cn

C#:   list.Contains(x)
来源：http://slb.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://nym.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ifk.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qab.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dgy.ydzc1.top

TS:   [...arr];
来源：http://llg.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://iwp.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ofo.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://xle.xuanzx.com

C#:   new List<int>(list);
来源：http://vnw.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://uub.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fde.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://duk.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfy.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ajp.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mim.yj20258888.top

Go:   // 手写循环
来源：http://vvz.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jkp.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rxy.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://mhx.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vwe.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pcm.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpy.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyw.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ejy.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oey.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dzs.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nhm.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://mzn.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://agg.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sbw.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vce.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nrh.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aiu.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://csw.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vqm.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hkw.xuetiantiany.cn

[D26] 数组转字符串
来源：http://kjg.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://oeo.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://xnx.jiagoushi.top

JS:   arr.join(", ")
来源：http://rvl.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://xku.yuxming.cn

Java: String.join(", ", list)
来源：http://rnv.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://nyn.shzxlz.cn

Ruby: arr.join(", ")
来源：http://rbp.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://apu.aibaodan.cn

================================================================================
来源：http://kwq.sjlbkw.cn

E. 字符串处理
来源：http://vlf.xingfuxueyuan.xyz

================================================================================
来源：http://iro.pycfn.com

[E01] 拼接字符串
来源：http://ywt.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jqo.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jca.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jgj.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfj.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vxf.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ljs.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://csl.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rmg.sxryk.cn

[E02] 重复字符串
来源：http://blg.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://kmz.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://idj.yonumen.top

JS:   "ab".repeat(3)
来源：http://reh.ybcxt.top

TS:   "ab".repeat(3)
来源：http://rtf.c1oappe.top

Java: "ab".repeat(3)
来源：http://tax.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://bjy.uphjek.com

Ruby: "ab" * 3
来源：http://pvi.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fim.yj202588.top

[E03] 截取子串
来源：http://jlp.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfz.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xhg.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tqj.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://omy.zhengqikj.top

Java: s.substring(1, 4)
来源：http://uvl.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uxo.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://wzv.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://btc.iojbl.cn

[E04] 查找子串位置
来源：http://qtj.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://lhj.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://wau.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xgo.52xcode.cn

TS:   s.indexOf("x")
来源：http://sew.ivvv.top

Java: s.indexOf("x")
来源：http://vzy.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://jhw.tianlin.xyz

Ruby: s.index("x")
来源：http://gsg.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://lul.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ogj.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iky.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lsq.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jvb.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uid.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uey.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rqa.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fli.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ujo.guannengcc.top

[E06] 替换子串
来源：http://bpy.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ybe.9152youxi.cn

PHP:  str_replace("a", "b", $s);
来源：http://wen.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ncd.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://aqx.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uuq.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mrg.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nfs.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://cyt.chenzaomai.com

[E07] 按分隔符拆分
来源：http://mzz.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lir.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://glu.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xma.hfpthk.cn

TS:   s.split(",")
来源：http://xfh.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://pgc.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kvm.yj202588.top

Ruby: s.split(",");  s.split
来源：http://sdn.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lps.daria6918.cn

[E08] 数组按分隔符合并
来源：http://nmh.xylfe.cn

Py:   ",".join(items)
来源：http://msh.iojbl.cn

PHP:  implode(",", $items);
来源：http://wom.hongshengwenyu.top

JS:   items.join(",")
来源：http://ffr.xylfe.cn

TS:   items.join(",")
来源：http://qtg.daxiang520.top

Java: String.join(",", items)
来源：http://hyx.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://zfw.chenlongwang.top

Ruby: items.join(",")
来源：http://asp.9152youxi.cn

C#:   string.Join(",", items)
来源：http://xah.chenlongwang.top

[E09] 去除所有空白字符
来源：http://lsr.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ilq.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xdf.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://fjb.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://kdy.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://jsc.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tyw.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sjv.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://idi.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://emk.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hna.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zaq.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://ghc.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://blh.tian-w.cn

Java: String.format("%03d", 7)
来源：http://xbv.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gkl.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hey.smart0.xyz


<!-- 参考信息 -->