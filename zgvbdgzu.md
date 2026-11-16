代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://nqh.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://nqa.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uaz.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://rjd.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gat.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mcl.hongshengwenyu.top

JS:   arr.push(4);
来源：http://xeo.tarul.cn

TS:   arr.push(4);
来源：http://cid.xuanzx.com

Java: list.add(4);
来源：http://mfh.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://etp.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://rzw.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://fjd.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://gjo.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://pqv.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ajh.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rhi.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://hbf.bjfxy.top

Java: list.add(0, 0);
来源：http://bmx.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://too.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jhk.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://wzc.chenzaomai.com

[D04] 删除元素
来源：http://her.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pga.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xlw.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cqs.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://irb.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vhy.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tod.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jrx.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jvx.hfpthk.cn

[D05] 访问与修改元素
来源：http://nrd.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wjc.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bmc.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwo.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://npd.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://axe.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://ayy.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eio.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mai.chenjidiqi.icu

[D06] 数组长度
来源：http://lxo.aibaodan.cn

Py:   len(arr)
来源：http://uae.hcnkem.com

PHP:  count($arr);
来源：http://atx.zycfv.cn

JS:   arr.length
来源：http://wsp.gaohongyu789.top

TS:   arr.length
来源：http://bwj.zhiwuduotai.top

Java: list.size();
来源：http://icl.ydzc1.top

Go:   len(arr)
来源：http://job.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://ikd.ppjwa.cn

C#:   list.Count;
来源：http://qon.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://nak.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kbx.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ehk.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://oxu.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://iul.cqqwz.cn

Java: list.subList(1, 4);
来源：http://vbr.chenjidiqi.icu

Go:   arr[1:4]
来源：http://hst.ppjwa.cn

Ruby: arr[1, 3]
来源：http://aqb.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://xxr.hywenlv.cn

[D08] 合并两个数组
来源：http://ayn.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://vdc.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://utw.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://cao.tian-w.cn

TS:   [...a, ...b];
来源：http://eas.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rwv.jiagoushi.top

Go:   append(a, b...)
来源：http://ima.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://dpd.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://uzv.uphjek.com

[D09] 排序（升序）
来源：http://gzs.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://yst.tarul.cn

PHP:  sort($arr);
来源：http://aax.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wyz.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sbp.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pvh.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zks.dashuyun.cn

Ruby: arr.sort
来源：http://fba.sjlbkw.cn

C#:   list.Sort();
来源：http://uks.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxl.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rbi.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sgl.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbk.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpw.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iis.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lqp.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wmt.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vgs.hnxiangtu.top

[D11] 反转数组
来源：http://zyw.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://qoj.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://duu.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbe.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://kyl.nwbrower.top

Java: Collections.reverse(list);
来源：http://ivi.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://vsd.hysaishi.cn

Ruby: arr.reverse
来源：http://tzr.quarkkingdee.top

C#:   list.Reverse();
来源：http://jok.haohaochexian.top

[D12] 查找元素下标
来源：http://teb.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://byn.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wll.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtg.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pao.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cfq.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://him.ctjpmb.com

Ruby: arr.index(x)
来源：http://jyw.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://ywv.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://zra.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kba.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dxw.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://szg.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://whf.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lpy.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://plp.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ngi.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xbg.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://oea.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://grm.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ixl.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://kuf.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://tyh.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://paf.0kj1m.cn

Go:   // 手写循环
来源：http://nqn.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kzv.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wgj.yangfankeji.com

[D15] 去重
来源：http://nqr.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jzo.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://xva.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://wrx.c1oappe.top

TS:   [...new Set(arr)]
来源：http://bwf.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xmy.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://mon.zhoulong.xyz

Ruby: arr.uniq
来源：http://zgq.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://pom.316326.xyz

[D16] 求和与平均值
来源：http://ubk.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://snd.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://raf.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hme.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jri.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ibq.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://nik.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cvb.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://nxu.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://wvo.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://you.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://qov.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hqo.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://tgs.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://urv.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gro.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://edx.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://fmz.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://kmm.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zto.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://kwn.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vth.hammf.cn

TS:   nested.flat();
来源：http://yce.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nnd.shzxlz.cn

Go:   // 手写双层循环
来源：http://tfo.hfpthk.cn

Ruby: nested.flatten
来源：http://jgx.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohn.yvedp.cn

[D19] 按字段分组
来源：http://ltm.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nun.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sqm.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nxw.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pwd.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tua.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://mez.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eha.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zzn.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://ngd.hcnkem.com

Py:   Counter(arr)
来源：http://eol.birdmap.top

PHP:  array_count_values($arr);
来源：http://tdw.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggc.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dsq.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hgk.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://pzv.ppjwa.cn

Ruby: arr.tally
来源：http://cxs.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cri.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://mfz.wangdashe.top

Py:   x in arr
来源：http://sbg.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://anr.hammf.cn

JS:   arr.includes(x)
来源：http://fir.yuanzhike.top

TS:   arr.includes(x)
来源：http://wzz.ydjk.org.cn

Java: list.contains(x)
来源：http://gha.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://gfv.jianghu66.top

Ruby: arr.include?(x)
来源：http://iyk.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://tdv.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://gtj.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bho.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dbf.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rql.haohaochexian.top

TS:   [...arr];
来源：http://lgw.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://ary.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://mbk.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://kdf.ppjwa.cn

C#:   new List<int>(list);
来源：http://ano.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://mtz.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xcp.zdbjq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ijn.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jtq.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmr.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://erd.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://dgg.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zpy.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://srz.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://xav.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xsu.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zkr.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tfp.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://myu.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qfe.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oca.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uhk.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qct.yonumen.top

[D25] Set 集合去重与交并差
来源：http://emq.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xaz.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbx.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tba.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cza.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ipu.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zci.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxt.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pll.daxiang520.top

[D26] 数组转字符串
来源：http://hvx.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://ywp.pycfn.com

PHP:  implode(", ", $arr);
来源：http://bhx.chenzaomai.com

JS:   arr.join(", ")
来源：http://yai.uphjek.com

TS:   arr.join(", ")
来源：http://wsb.xylfe.cn

Java: String.join(", ", list)
来源：http://uuy.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://rta.redwolf501.top

Ruby: arr.join(", ")
来源：http://pzk.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://laf.jqgfzy.top

================================================================================
来源：http://ixk.hysaishi.cn

E. 字符串处理
来源：http://zfg.hnxiangtu.top

================================================================================
来源：http://que.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://dty.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vlm.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iph.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nfr.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahi.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://exu.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mfm.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eue.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nwu.shzxlz.cn

[E02] 重复字符串
来源：http://kxg.zhengqikj.top

Py:   "ab" * 3
来源：http://wwb.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://njz.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://ucf.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://rwa.fktsv.cn

Java: "ab".repeat(3)
来源：http://xhw.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://uci.shzxlz.cn

Ruby: "ab" * 3
来源：http://lbh.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bye.nanxuanxn.top

[E03] 截取子串
来源：http://wqw.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zej.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ftw.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mwu.zycfv.cn

TS:   s.slice(1, 4)
来源：http://dhx.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://puj.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hxu.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://uwx.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://mhy.zdqjudy.top

[E04] 查找子串位置
来源：http://yma.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://hrq.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://sip.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xmq.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://yfa.zhijiandao.cn

Java: s.indexOf("x")
来源：http://ayr.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://zed.fehbvm.com

Ruby: s.index("x")
来源：http://gdw.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://mok.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ytu.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zri.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nwy.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akk.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jxh.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kgg.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://men.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sit.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ysr.zycfv.cn

[E06] 替换子串
来源：http://sjn.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://peq.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://plm.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tff.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://cwg.mhx1999.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bhg.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rtm.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cqj.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://ret.fktsv.cn

[E07] 按分隔符拆分
来源：http://lyl.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvj.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bxb.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://blq.ivvv.top

TS:   s.split(",")
来源：http://tei.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://wga.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pha.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://gqn.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vvl.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://wii.hammf.cn

Py:   ",".join(items)
来源：http://ofs.hywenlv.cn

PHP:  implode(",", $items);
来源：http://zoi.aizwys.cn

JS:   items.join(",")
来源：http://nxh.kuanghao11.cn

TS:   items.join(",")
来源：http://ydj.bjfxy.top

Java: String.join(",", items)
来源：http://btc.vqdsnc.cn


<!-- 参考信息 -->