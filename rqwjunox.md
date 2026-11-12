代发 wailian999

Java: list.add(4);
来源：http://iso.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://wsw.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://bwc.dianchejie.cn

C#:   list.Add(4);
来源：http://uvz.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://dww.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://lsh.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://amj.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ghx.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://kji.jianghu66.top

Java: list.add(0, 0);
来源：http://ojb.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jrz.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aht.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://bjt.epnwcf.com

[D04] 删除元素
来源：http://ans.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dru.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tcs.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jmp.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://wxm.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lid.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mxn.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://som.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wcn.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://iko.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tnb.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gdb.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jzo.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://dtn.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://jid.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://zhb.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lci.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wfk.chenjidiqi.icu

[D06] 数组长度
来源：http://fcp.jqgufenzy.top

Py:   len(arr)
来源：http://rwn.vehdjk.com

PHP:  count($arr);
来源：http://akx.vqdsnc.cn

JS:   arr.length
来源：http://ajc.chenzaomai.com

TS:   arr.length
来源：http://xtw.52xcode.cn

Java: list.size();
来源：http://eea.zycfv.cn

Go:   len(arr)
来源：http://mxb.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://hzg.hcnkem.com

C#:   list.Count;
来源：http://rwc.hammf.cn

[D07] 切片 / 取子数组
来源：http://tvw.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tra.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://efx.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://yua.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://mwa.yj20258.top

Java: list.subList(1, 4);
来源：http://aay.hcnkem.com

Go:   arr[1:4]
来源：http://llx.fehbvm.com

Ruby: arr[1, 3]
来源：http://ljr.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://eny.hysaishi.cn

[D08] 合并两个数组
来源：http://dik.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://izo.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://xln.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bmo.wangdashe.top

TS:   [...a, ...b];
来源：http://vks.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://muk.andypj.xyz

Go:   append(a, b...)
来源：http://ild.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://vsp.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://rgu.yuanzhike.top

[D09] 排序（升序）
来源：http://xje.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgu.fktsv.cn

PHP:  sort($arr);
来源：http://tmz.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://beo.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://til.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wad.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eii.jinghuilouyu.cn

Ruby: arr.sort
来源：http://myv.fzhhl.top

C#:   list.Sort();
来源：http://mbi.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://elr.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dzy.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iiu.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpj.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mrt.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nxl.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://owi.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vfb.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kgo.zhoulong.xyz

[D11] 反转数组
来源：http://qda.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://fet.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://lei.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lui.c1oappe.top

TS:   [...arr].reverse();
来源：http://vdw.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://xsw.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://tuc.hcnkem.com

Ruby: arr.reverse
来源：http://yvd.sxryk.cn

C#:   list.Reverse();
来源：http://eoq.zhiwuduotai.top

[D12] 查找元素下标
来源：http://vjs.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://xnp.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lfy.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eeh.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tui.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aii.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://nlx.haohaochexian.top

Ruby: arr.index(x)
来源：http://uul.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://hza.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://llp.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lqg.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gcp.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://nmz.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://gcr.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nnj.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://chr.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://jpr.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eii.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://vxl.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xqi.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vjy.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://tmj.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://dyq.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lah.gogol.net.cn

Go:   // 手写循环
来源：http://pfl.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qkq.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ifq.yangfankeji.com

[D15] 去重
来源：http://prp.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mec.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://otd.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://xze.yonumen.top

TS:   [...new Set(arr)]
来源：http://exj.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rkm.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rfq.hysaishi.cn

Ruby: arr.uniq
来源：http://yiw.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://zih.feifeiyinyue.top

[D16] 求和与平均值
来源：http://yoz.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://udt.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jiq.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ngv.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gpc.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpr.gaohongyu789.top

Go:   // 手写循环累加
来源：http://gmq.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ofi.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://snz.smart0.xyz

[D17] 最大值与最小值
来源：http://qfq.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://rks.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://liz.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rce.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://pzc.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hel.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://guu.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://btf.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://wgn.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://xot.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://khz.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://utg.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ekx.vehdjk.com

TS:   nested.flat();
来源：http://gmn.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ndd.aizwys.cn

Go:   // 手写双层循环
来源：http://sxn.iojbl.cn

Ruby: nested.flatten
来源：http://spy.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://wmi.hesvh.cn

[D19] 按字段分组
来源：http://qcb.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rxq.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmo.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qff.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://vhb.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://arr.yonumen.top

Go:   // 手写 map[string][]T
来源：http://wrw.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://efn.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hxw.birdmap.top

[D20] 统计每个元素出现次数
来源：http://bpt.hnxiangtu.top

Py:   Counter(arr)
来源：http://xex.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://zcq.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://spf.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rau.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mzl.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://psn.cucudq.cn

Ruby: arr.tally
来源：http://yyy.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzk.hammf.cn

[D21] 判断是否包含某元素
来源：http://mbf.gzhubu.top

Py:   x in arr
来源：http://zjr.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://gfk.shuidangran.top

JS:   arr.includes(x)
来源：http://avr.yvedp.cn

TS:   arr.includes(x)
来源：http://yjj.yongpay.top

Java: list.contains(x)
来源：http://gyv.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://ago.hcnkem.com

Ruby: arr.include?(x)
来源：http://dmz.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://epf.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://ojv.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lzt.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gif.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bdj.ctjpmb.com

TS:   [...arr];
来源：http://xcg.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://wiu.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qyy.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://qpy.ybcxt.top

C#:   new List<int>(list);
来源：http://hil.zdqjudy.top

[D23] reduce 累积计算
来源：http://pkq.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uya.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ypl.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hoh.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xul.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mqn.mhx1999.top

Go:   // 手写循环
来源：http://etz.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vsr.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nat.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://vie.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mxv.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hqa.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ama.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nlg.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wpc.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cec.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hjh.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pvk.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://oaw.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whk.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ccy.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbg.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kni.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zol.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jhc.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ymu.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cng.yongpay.top

[D26] 数组转字符串
来源：http://lhw.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://pbi.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://fly.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://gxp.meibo888.top

TS:   arr.join(", ")
来源：http://miu.meibo888.top

Java: String.join(", ", list)
来源：http://uwe.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://hjj.birdmap.top

Ruby: arr.join(", ")
来源：http://apx.hesvh.cn

C#:   string.Join(", ", list)
来源：http://vca.shuidangran.top

================================================================================
来源：http://pxw.sweek.top

E. 字符串处理
来源：http://prb.jinyuanbaomall.cn

================================================================================
来源：http://njt.meibo888.top

[E01] 拼接字符串
来源：http://wmw.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xcp.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://arf.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vot.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmt.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xge.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yma.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://epv.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rsf.tian-w.cn

[E02] 重复字符串
来源：http://uph.hysaishi.cn

Py:   "ab" * 3
来源：http://guo.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://eff.andypj.xyz

JS:   "ab".repeat(3)
来源：http://yne.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://uba.shuidangran.top

Java: "ab".repeat(3)
来源：http://hdn.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://wtg.sufxvd.cn

Ruby: "ab" * 3
来源：http://ymh.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sha.xuetiantiany.cn

[E03] 截取子串
来源：http://yhq.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jao.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxx.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fwn.bjfxy.top

TS:   s.slice(1, 4)
来源：http://rlm.daxiang520.top

Java: s.substring(1, 4)
来源：http://yxk.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gqd.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://drg.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://vui.wangshuangyany.cn

[E04] 查找子串位置
来源：http://xwg.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://mbm.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://jef.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jsa.fengsongda.top

TS:   s.indexOf("x")
来源：http://sun.uphjek.com

Java: s.indexOf("x")
来源：http://fox.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://ykw.daxiang520.top

Ruby: s.index("x")
来源：http://pwq.shuidangran.top

C#:   s.IndexOf("x")
来源：http://clt.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aid.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qrr.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qjj.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mgk.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gva.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhv.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qtl.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aed.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fzy.52xcode.cn

[E06] 替换子串
来源：http://otm.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ytl.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ntx.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://evg.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://xqo.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gnx.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rdr.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mbg.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://wfi.ctjpmb.com

[E07] 按分隔符拆分
来源：http://qpk.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qjc.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oay.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://idl.hongshengwenyu.top

TS:   s.split(",")
来源：http://tnn.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://pjd.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://smj.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://vom.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iik.tarul.cn

[E08] 数组按分隔符合并
来源：http://trg.hfpthk.cn

Py:   ",".join(items)
来源：http://mkr.jinqigufen.top

PHP:  implode(",", $items);
来源：http://jyb.cashguo.top

JS:   items.join(",")
来源：http://wyz.fanxiaobao.xyz

TS:   items.join(",")
来源：http://uyy.9152youxi.cn

Java: String.join(",", items)
来源：http://tkx.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://kfp.havefunace.top

Ruby: items.join(",")
来源：http://rsy.52xcode.cn

C#:   string.Join(",", items)
来源：http://afa.zycfv.cn

[E09] 去除所有空白字符
来源：http://ggl.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjd.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfq.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://hpd.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://htz.9152youxi.cn


<!-- 参考信息 -->