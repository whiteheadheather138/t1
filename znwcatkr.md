代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mjf.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nxo.jlsjyb.cn

JS:   arr.push(4);
来源：http://dnx.zhixingplan.top

TS:   arr.push(4);
来源：http://wxp.fanxiaobao.xyz

Java: list.add(4);
来源：http://mkz.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://vyj.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://xva.jinqigufen.top

C#:   list.Add(4);
来源：http://htq.hammf.cn

[D03] 在指定位置插入元素
来源：http://wjh.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://bbn.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://owy.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kgy.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://dpb.tianlin.xyz

Java: list.add(0, 0);
来源：http://jzm.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hyu.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://avr.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://hzg.hammf.cn

[D04] 删除元素
来源：http://muf.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://edi.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ckk.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://syu.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://its.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://geh.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://evc.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yia.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sax.9152youxi.cn

[D05] 访问与修改元素
来源：http://int.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qro.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ann.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ltd.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://umt.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ywd.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://igu.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nvp.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ddq.tarul.cn

[D06] 数组长度
来源：http://vjq.nwbrower.top

Py:   len(arr)
来源：http://taj.guannengcc.top

PHP:  count($arr);
来源：http://fmn.tianlin.xyz

JS:   arr.length
来源：http://cqe.cucudq.cn

TS:   arr.length
来源：http://kmh.zhengqikj.top

Java: list.size();
来源：http://pax.jinghuilouyu.cn

Go:   len(arr)
来源：http://pkp.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://hww.zhiwuduotai.top

C#:   list.Count;
来源：http://lhd.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://tgt.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ndo.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://vkn.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://evf.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://dmi.dashuyun.cn

Java: list.subList(1, 4);
来源：http://xvc.hcnkem.com

Go:   arr[1:4]
来源：http://tle.ehwqpu.com

Ruby: arr[1, 3]
来源：http://chk.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://slc.jyoumei.cn

[D08] 合并两个数组
来源：http://gfj.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://iiu.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://rxt.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lrd.yangfankeji.com

TS:   [...a, ...b];
来源：http://mxe.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://viq.iojbl.cn

Go:   append(a, b...)
来源：http://ntj.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://lsd.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://osg.jyoumei.cn

[D09] 排序（升序）
来源：http://ovj.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hby.yangfankeji.com

PHP:  sort($arr);
来源：http://btj.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jtb.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rkt.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://roh.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lhn.zhixingplan.top

Ruby: arr.sort
来源：http://dcn.smart0.xyz

C#:   list.Sort();
来源：http://cyk.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zgc.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xwe.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://siy.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iaj.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vgx.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://acz.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://euv.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://shr.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://myt.hammf.cn

[D11] 反转数组
来源：http://quq.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://xob.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://isr.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hco.cqqwz.cn

TS:   [...arr].reverse();
来源：http://xms.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://ofp.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://zbv.jinqigufen.top

Ruby: arr.reverse
来源：http://sfz.dashuyun.cn

C#:   list.Reverse();
来源：http://tsu.quarkkingdee.top

[D12] 查找元素下标
来源：http://qwf.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://jlb.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wsa.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emt.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://olg.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sjr.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://pou.bbcook.cn

Ruby: arr.index(x)
来源：http://pbk.ybcxt.top

C#:   list.IndexOf(x);
来源：http://rga.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://lao.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uuz.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fcg.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://reu.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://xft.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://czv.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfm.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yxy.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oyx.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://gej.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qqb.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://icv.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://smi.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://tgm.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vel.hywenlv.cn

Go:   // 手写循环
来源：http://cic.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uze.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://haf.yonumen.top

[D15] 去重
来源：http://pyj.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eip.0kj1m.cn

PHP:  array_unique($arr);
来源：http://fxe.fktsv.cn

JS:   [...new Set(arr)]
来源：http://xap.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://pnl.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jgj.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fib.xziqi.cn

Ruby: arr.uniq
来源：http://jrb.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://itd.jiagoushi.top

[D16] 求和与平均值
来源：http://kbl.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pzl.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ygg.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwp.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://frh.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yfa.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://ced.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nbi.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://zgr.sufxvd.cn

[D17] 最大值与最小值
来源：http://wzj.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://cwq.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://gmi.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yph.sweek.top

TS:   Math.max(...arr);
来源：http://bep.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ysj.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://avy.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://yfq.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://cjw.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://kqs.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hmg.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://iqi.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lyz.cashguo.top

TS:   nested.flat();
来源：http://jst.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://egp.gogol.net.cn

Go:   // 手写双层循环
来源：http://rwh.svipenyu.cn

Ruby: nested.flatten
来源：http://ifd.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lzx.pengpengdd.cyou

[D19] 按字段分组
来源：http://eny.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ktf.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vzk.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://faf.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bld.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gfp.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://kss.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xvc.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsf.yj20258.top

[D20] 统计每个元素出现次数
来源：http://lcu.yfazqb.com

Py:   Counter(arr)
来源：http://hlf.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://qks.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zya.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://snd.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://daa.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://nnv.cdnleiting.top

Ruby: arr.tally
来源：http://mmm.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xaz.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://efw.yj20258888.top

Py:   x in arr
来源：http://nhr.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://ckw.xylfe.cn

JS:   arr.includes(x)
来源：http://hmf.52xcode.cn

TS:   arr.includes(x)
来源：http://zfk.vqdsnc.cn

Java: list.contains(x)
来源：http://ssg.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://mwj.sweek.top

Ruby: arr.include?(x)
来源：http://onc.vehdjk.com

C#:   list.Contains(x)
来源：http://yab.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://wfi.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vpc.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ynd.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nbj.yuxming.cn

TS:   [...arr];
来源：http://ysq.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://thb.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://gna.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://orj.yuxming.cn

C#:   new List<int>(list);
来源：http://lbl.yj202588.top

[D23] reduce 累积计算
来源：http://ssn.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nqt.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bxz.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hsj.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cni.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qbi.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://spv.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hmx.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iys.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://rzu.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://izl.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://snm.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fuf.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ske.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://smk.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fbr.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jud.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dzq.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://bxy.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hdp.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tun.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ufm.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zzc.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://upm.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ppt.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gvp.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zel.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://rux.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://rnb.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://dpn.snrcjt.cn

JS:   arr.join(", ")
来源：http://ahq.cucudq.cn

TS:   arr.join(", ")
来源：http://qum.nwbrower.top

Java: String.join(", ", list)
来源：http://dcg.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://euh.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://iyf.52xcode.cn

C#:   string.Join(", ", list)
来源：http://qlr.mhx1999.top

================================================================================
来源：http://nat.xinyue.icu

E. 字符串处理
来源：http://xsa.hnxiangtu.top

================================================================================
来源：http://ink.316326.xyz

[E01] 拼接字符串
来源：http://vvp.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cet.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gcg.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkq.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hlw.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sws.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ovx.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nnt.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rvs.xylfe.cn

[E02] 重复字符串
来源：http://cxc.cdnleiting.top

Py:   "ab" * 3
来源：http://ztt.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://otn.ivvv.top

JS:   "ab".repeat(3)
来源：http://ryh.yj20258.top

TS:   "ab".repeat(3)
来源：http://dmu.gotoacloud.top

Java: "ab".repeat(3)
来源：http://qby.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://fwo.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://req.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uww.ppjwa.cn

[E03] 截取子串
来源：http://hsv.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyy.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hrz.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jxw.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://ddj.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://xlj.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bdr.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://bhx.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://gqt.haohaochexian.top

[E04] 查找子串位置
来源：http://nkn.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://ael.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://gdl.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ovk.0kj1m.cn

TS:   s.indexOf("x")
来源：http://aae.yuanzhike.top

Java: s.indexOf("x")
来源：http://yrh.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://swi.ppjwa.cn

Ruby: s.index("x")
来源：http://ttx.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://wuv.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kav.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cfv.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oee.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxv.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hsw.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nfa.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://slx.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hxw.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gen.guannengcc.top

[E06] 替换子串
来源：http://cjd.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://onr.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://lhf.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://skx.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://cxu.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tua.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://knt.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yfi.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://gcx.havefunace.top

[E07] 按分隔符拆分
来源：http://vvg.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wyh.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xcl.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ulw.chenzaomai.com

TS:   s.split(",")
来源：http://rsh.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://sjf.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tuk.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://egf.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kqc.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://dip.andypj.xyz

Py:   ",".join(items)
来源：http://vzt.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://zce.xinyue.icu

JS:   items.join(",")
来源：http://kts.fktsv.cn

TS:   items.join(",")
来源：http://uvn.jqgfzy.top

Java: String.join(",", items)
来源：http://edm.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://cmk.fehbvm.com

Ruby: items.join(",")
来源：http://zbn.fktsv.cn

C#:   string.Join(",", items)
来源：http://jve.yj202588.top

[E09] 去除所有空白字符
来源：http://gnx.aizwys.cn


<!-- 参考信息 -->