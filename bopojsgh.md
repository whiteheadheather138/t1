代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://dph.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://yeh.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xkp.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://isz.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dmw.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vxb.ybcxt.top

JS:   arr.push(4);
来源：http://yos.52xcode.cn

TS:   arr.push(4);
来源：http://pgu.jlsjyb.cn

Java: list.add(4);
来源：http://zpx.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://yjs.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://naz.fktsv.cn

C#:   list.Add(4);
来源：http://ikz.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://gaf.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://egp.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ndk.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uue.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://kfu.cqqwz.cn

Java: list.add(0, 0);
来源：http://jji.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zai.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fbz.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://tiv.tanke756.top

[D04] 删除元素
来源：http://ytv.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://asp.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://akq.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dyi.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://hyc.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://meb.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dit.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wxk.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mhb.cheryme.top

[D05] 访问与修改元素
来源：http://avr.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfc.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gls.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uht.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://awq.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://tpf.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://caq.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sbe.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hnp.gzhubu.top

[D06] 数组长度
来源：http://rce.haohaochexian.top

Py:   len(arr)
来源：http://kdu.hongshengwenyu.top

PHP:  count($arr);
来源：http://jpb.yanxiufei.cn

JS:   arr.length
来源：http://ftp.ehwqpu.com

TS:   arr.length
来源：http://wdu.zhijiandao.cn

Java: list.size();
来源：http://ssr.yanxiufei.cn

Go:   len(arr)
来源：http://jte.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://oqr.hnxiangtu.top

C#:   list.Count;
来源：http://wgk.nwbrower.top

[D07] 切片 / 取子数组
来源：http://uob.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dfc.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zyk.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://mcd.yongpay.top

TS:   arr.slice(1, 4);
来源：http://eff.0kj1m.cn

Java: list.subList(1, 4);
来源：http://vpx.chenlongwang.top

Go:   arr[1:4]
来源：http://rdh.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://okb.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://lpi.c1oappe.top

[D08] 合并两个数组
来源：http://ytn.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://phf.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://qqz.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://oqg.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://ehr.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uhg.jinqigfzy.top

Go:   append(a, b...)
来源：http://zme.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://ehu.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://gwv.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://vxb.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://hts.shangyingyoupin.top

PHP:  sort($arr);
来源：http://tgz.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qij.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tkm.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qrv.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bzo.fengsongda.top

Ruby: arr.sort
来源：http://nfe.hcnkem.com

C#:   list.Sort();
来源：http://rfi.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://gzm.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyp.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eyu.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zst.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tdx.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://moj.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://itq.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mrw.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dli.yj202588.top

[D11] 反转数组
来源：http://vzl.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hyy.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://kqs.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfa.ehwqpu.com

TS:   [...arr].reverse();
来源：http://kza.aibaodan.cn

Java: Collections.reverse(list);
来源：http://ehz.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://mkh.guowangkeji.top

Ruby: arr.reverse
来源：http://ipf.ydjk.org.cn

C#:   list.Reverse();
来源：http://zaj.cdnleiting.top

[D12] 查找元素下标
来源：http://ovu.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://ven.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tkc.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ede.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://guz.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kme.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://onn.hammf.cn

Ruby: arr.index(x)
来源：http://oen.52xcode.cn

C#:   list.IndexOf(x);
来源：http://xeu.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://eby.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://obu.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://prw.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://msj.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://zeo.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rfn.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rke.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://tib.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hhk.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://tfo.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jkt.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dvj.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://wsz.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://yvl.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfu.hammf.cn

Go:   // 手写循环
来源：http://qwx.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://kly.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://utc.chenjidiqi.icu

[D15] 去重
来源：http://dtx.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://exv.zhengqikj.top

PHP:  array_unique($arr);
来源：http://bwd.daxiang520.top

JS:   [...new Set(arr)]
来源：http://cwx.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://rlk.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xdb.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tkg.yuanzhike.top

Ruby: arr.uniq
来源：http://cwo.uphjek.com

C#:   list.Distinct().ToList()
来源：http://rsm.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://qds.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://god.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://igq.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sfj.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vlh.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fkg.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://scb.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://skf.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://hci.vehdjk.com

[D17] 最大值与最小值
来源：http://cvk.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://spt.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://pku.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hne.jiagoushi.top

TS:   Math.max(...arr);
来源：http://kgo.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oiw.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cmw.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://xaj.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://djl.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://pxe.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fxh.tarul.cn

PHP:  array_merge(...$nested);
来源：http://jki.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://quz.kuanghao11.cn

TS:   nested.flat();
来源：http://dij.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://odu.havefunace.top

Go:   // 手写双层循环
来源：http://xin.havefunace.top

Ruby: nested.flatten
来源：http://puy.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://drf.pycfn.com

[D19] 按字段分组
来源：http://mne.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nhi.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gag.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uxo.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwa.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cpi.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://rda.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yat.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qsz.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://oio.sufxvd.cn

Py:   Counter(arr)
来源：http://djr.hammf.cn

PHP:  array_count_values($arr);
来源：http://tkd.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgx.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vcf.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lnr.ivvv.top

Go:   // 手写 map[T]int
来源：http://jpc.dashuyun.cn

Ruby: arr.tally
来源：http://fxz.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mke.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://frc.chenzaomai.com

Py:   x in arr
来源：http://gjx.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://bis.xinyue.icu

JS:   arr.includes(x)
来源：http://enk.tarul.cn

TS:   arr.includes(x)
来源：http://jla.yonumen.top

Java: list.contains(x)
来源：http://giq.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://sim.fengsongda.top

Ruby: arr.include?(x)
来源：http://ojc.svipenyu.cn

C#:   list.Contains(x)
来源：http://jza.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://wzj.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sbj.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tan.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zsu.yongpay.top

TS:   [...arr];
来源：http://hxm.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://uhu.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fvw.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://fyg.yangfankeji.com

C#:   new List<int>(list);
来源：http://ngw.jiagoushi.top

[D23] reduce 累积计算
来源：http://fhm.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sww.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wdu.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qmj.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbf.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vrk.wangdashe.top

Go:   // 手写循环
来源：http://nwx.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hwi.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hht.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://ndy.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bpy.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xgk.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://egm.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hkp.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wpk.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vos.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oap.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ygx.birdmap.top

[D25] Set 集合去重与交并差
来源：http://yxt.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://too.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://diz.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bxo.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aap.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wxo.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cgi.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dbx.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ote.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://ycq.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://mfh.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://ewi.tian-w.cn

JS:   arr.join(", ")
来源：http://qfi.jinqigufen.top

TS:   arr.join(", ")
来源：http://iyb.xziqi.cn

Java: String.join(", ", list)
来源：http://aas.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://yaz.chenzaomai.com

Ruby: arr.join(", ")
来源：http://iyl.sxryk.cn

C#:   string.Join(", ", list)
来源：http://adr.yonumen.top

================================================================================
来源：http://gwb.haohaochexian.top

E. 字符串处理
来源：http://fel.jqgufenzy.top

================================================================================
来源：http://qjm.feifeiyinyue.top

[E01] 拼接字符串
来源：http://iqb.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yuc.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vpd.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qiw.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jxw.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wsk.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ytb.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rmt.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ifs.tarul.cn

[E02] 重复字符串
来源：http://hfk.316326.xyz

Py:   "ab" * 3
来源：http://gks.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://bqr.cashguo.top

JS:   "ab".repeat(3)
来源：http://tje.redwolf501.top

TS:   "ab".repeat(3)
来源：http://wof.yuxming.cn

Java: "ab".repeat(3)
来源：http://frw.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://qse.xinyue.icu

Ruby: "ab" * 3
来源：http://hlh.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqj.jinqigufen.top

[E03] 截取子串
来源：http://all.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://emw.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tql.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wyx.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://gkh.meibo888.top

Java: s.substring(1, 4)
来源：http://wof.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cfo.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://jkk.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://jhd.jlsjyb.cn

[E04] 查找子串位置
来源：http://zqy.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://whh.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://wif.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://est.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://aol.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://dee.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://lsr.c1oappe.top

Ruby: s.index("x")
来源：http://yuu.ivvv.top

C#:   s.IndexOf("x")
来源：http://zds.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://uxq.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cov.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://myz.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gzi.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjx.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoy.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uom.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ltn.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xvq.daria6918.cn

[E06] 替换子串
来源：http://trm.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fxt.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://xcy.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyt.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://rok.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhy.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ppp.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wzz.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://mdq.yonumen.top

[E07] 按分隔符拆分
来源：http://tho.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nqs.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bsv.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hlj.kuanghao11.cn

TS:   s.split(",")
来源：http://drs.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://jwo.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://utp.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://bno.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qmd.xinyue.icu

[E08] 数组按分隔符合并
来源：http://fsy.feifeiyinyue.top

Py:   ",".join(items)
来源：http://tjx.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://oks.guowangkeji.top

JS:   items.join(",")
来源：http://wcu.ctjpmb.com

TS:   items.join(",")
来源：http://wnc.nanxuanxn.top

Java: String.join(",", items)
来源：http://qgo.fzhhl.top


<!-- 参考信息 -->