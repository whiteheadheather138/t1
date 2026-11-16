代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qzo.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://urq.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vci.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmg.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://wmb.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://unu.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nby.yongpay.top

[D02] 追加元素到末尾
来源：http://xpl.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://avg.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bgx.mhx1999.top

JS:   arr.push(4);
来源：http://tjo.wangdashe.top

TS:   arr.push(4);
来源：http://rui.hywenlv.cn

Java: list.add(4);
来源：http://ddw.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://rkn.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://ncq.ydzc1.top

C#:   list.Add(4);
来源：http://tiw.daria6918.cn

[D03] 在指定位置插入元素
来源：http://cvq.yonumen.top

Py:   arr.insert(0, 0)
来源：http://uom.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://giz.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://swz.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://sug.snrcjt.cn

Java: list.add(0, 0);
来源：http://nnr.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ntb.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zyi.birdmap.top

C#:   list.Insert(0, 0);
来源：http://bzj.shzxlz.cn

[D04] 删除元素
来源：http://fwo.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sqc.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mog.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qtg.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://ocj.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://beq.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://snw.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vee.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wtv.hnqzz.top

[D05] 访问与修改元素
来源：http://oyo.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pda.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jdp.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sob.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://evv.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://mfe.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://gvt.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oxo.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kpr.tianlin.xyz

[D06] 数组长度
来源：http://zoq.bjfxy.top

Py:   len(arr)
来源：http://wbb.xuanzx.com

PHP:  count($arr);
来源：http://htj.zhaomingkeji.xyz

JS:   arr.length
来源：http://ujn.ydjk.org.cn

TS:   arr.length
来源：http://qiy.hfpthk.cn

Java: list.size();
来源：http://vhf.dashuyun.cn

Go:   len(arr)
来源：http://uvs.52xcode.cn

Ruby: arr.length; arr.size
来源：http://lop.jqgufenzy.top

C#:   list.Count;
来源：http://hfg.sxryk.cn

[D07] 切片 / 取子数组
来源：http://dxo.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pwj.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://lgk.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://ata.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://mqn.yangfankeji.com

Java: list.subList(1, 4);
来源：http://dwz.bjfxy.top

Go:   arr[1:4]
来源：http://udp.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://dkp.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://ilb.fengsongda.top

[D08] 合并两个数组
来源：http://mrl.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://gsh.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://ane.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mlj.yuxming.cn

TS:   [...a, ...b];
来源：http://ctq.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ytb.cashguo.top

Go:   append(a, b...)
来源：http://xtc.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://umt.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://dwd.sysykeji.top

[D09] 排序（升序）
来源：http://ues.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://izn.yuanzhike.top

PHP:  sort($arr);
来源：http://ikk.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nkz.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oif.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dof.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dbj.nanxuanxn.top

Ruby: arr.sort
来源：http://gsu.gzhubu.top

C#:   list.Sort();
来源：http://axg.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://drx.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zqu.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssh.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gnl.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfx.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://huk.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tuj.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qmj.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://egp.hysaishi.cn

[D11] 反转数组
来源：http://xdv.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://oip.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://yhn.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mnt.daria6918.cn

TS:   [...arr].reverse();
来源：http://qds.jianghu66.top

Java: Collections.reverse(list);
来源：http://dac.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://pyn.sjlbkw.cn

Ruby: arr.reverse
来源：http://uyz.svipenyu.cn

C#:   list.Reverse();
来源：http://zjv.yonumen.top

[D12] 查找元素下标
来源：http://qwd.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://ats.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fho.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epi.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dco.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jku.sweek.top

Go:   slices.Index(arr, x)
来源：http://qip.jinqigfzy.top

Ruby: arr.index(x)
来源：http://ebh.fengsongda.top

C#:   list.IndexOf(x);
来源：http://uxy.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://upn.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://duw.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cjq.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://rua.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://dzg.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lof.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://myb.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://flr.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yfg.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://tgp.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eio.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sto.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://oqd.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://dhw.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wdi.bbcook.cn

Go:   // 手写循环
来源：http://axi.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hch.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hwo.guannengcc.top

[D15] 去重
来源：http://ytz.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ryg.dianchejie.cn

PHP:  array_unique($arr);
来源：http://dxt.hnqzz.top

JS:   [...new Set(arr)]
来源：http://bow.epnwcf.com

TS:   [...new Set(arr)]
来源：http://isd.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vvb.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pcl.sysykeji.top

Ruby: arr.uniq
来源：http://aye.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://jam.zhongyouzk.top

[D16] 求和与平均值
来源：http://jvb.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gon.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kqa.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsc.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dvh.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tyn.havefunace.top

Go:   // 手写循环累加
来源：http://ais.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dup.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://mpf.quarkkingdee.top

[D17] 最大值与最小值
来源：http://fmp.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://etm.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://iqt.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bqf.redwolf501.top

TS:   Math.max(...arr);
来源：http://bbv.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ydh.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cdq.havefunace.top

Ruby: arr.max;  arr.min
来源：http://gub.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://kfj.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://suc.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ycs.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://xti.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://biu.tianlin.xyz

TS:   nested.flat();
来源：http://inm.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://faa.smart0.xyz

Go:   // 手写双层循环
来源：http://rgi.mhx1999.top

Ruby: nested.flatten
来源：http://oql.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hst.feifeiyinyue.top

[D19] 按字段分组
来源：http://pqs.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hoi.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qvc.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gji.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qox.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ipk.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://hyk.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zub.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sxw.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://bpw.jinqigufen.top

Py:   Counter(arr)
来源：http://yzs.cucudq.cn

PHP:  array_count_values($arr);
来源：http://wqr.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wre.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://box.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gyd.shuidangran.top

Go:   // 手写 map[T]int
来源：http://muw.redwolf501.top

Ruby: arr.tally
来源：http://ygs.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wzz.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://slk.ydzc1.top

Py:   x in arr
来源：http://gvr.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://nns.gaohongyu789.top

JS:   arr.includes(x)
来源：http://bpp.fengsongda.top

TS:   arr.includes(x)
来源：http://arv.redwolf501.top

Java: list.contains(x)
来源：http://msf.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://dzl.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://opy.jqgfzy.top

C#:   list.Contains(x)
来源：http://xba.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://nfs.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltr.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gsq.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uza.feifeiyinyue.top

TS:   [...arr];
来源：http://isl.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://tlt.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fqe.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://kpv.birdmap.top

C#:   new List<int>(list);
来源：http://uvd.yangfankeji.com

[D23] reduce 累积计算
来源：http://ztm.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://efx.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pif.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jap.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwh.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dap.shanyushiyangtech.top

Go:   // 手写循环
来源：http://fmv.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xta.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qhp.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://isn.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://djs.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gvu.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wmm.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zth.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pic.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eod.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nvn.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ikf.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://gwg.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hfd.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbu.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nsn.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cta.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vcx.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wlh.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://urw.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yem.aizwys.cn

[D26] 数组转字符串
来源：http://acb.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://fcj.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://uvb.ydjk.org.cn

JS:   arr.join(", ")
来源：http://oan.ivvv.top

TS:   arr.join(", ")
来源：http://uzr.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://dyi.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://phu.cashguo.top

Ruby: arr.join(", ")
来源：http://dia.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://wst.xuetiantiany.cn

================================================================================
来源：http://mmz.ppjwa.cn

E. 字符串处理
来源：http://ynb.meibo888.top

================================================================================
来源：http://elh.yangfankeji.com

[E01] 拼接字符串
来源：http://ndz.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aby.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pnm.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ffe.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xia.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pru.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ivo.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ots.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ubj.xuetiantiany.cn

[E02] 重复字符串
来源：http://ckz.tarul.cn

Py:   "ab" * 3
来源：http://bpq.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://app.pycfn.com

JS:   "ab".repeat(3)
来源：http://yse.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://vcf.yuxming.cn

Java: "ab".repeat(3)
来源：http://ohu.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://fsm.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://iov.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kce.sweek.top

[E03] 截取子串
来源：http://hqg.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gbb.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qgr.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xen.sysykeji.top

TS:   s.slice(1, 4)
来源：http://lfk.zdbjq.cn

Java: s.substring(1, 4)
来源：http://iro.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lcd.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://vsb.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://wcg.yonumen.top

[E04] 查找子串位置
来源：http://gln.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://deu.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://zbi.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cdv.hammf.cn

TS:   s.indexOf("x")
来源：http://hpm.zhijiandao.cn

Java: s.indexOf("x")
来源：http://zvn.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://jhc.smart0.xyz

Ruby: s.index("x")
来源：http://hna.tarul.cn

C#:   s.IndexOf("x")
来源：http://iru.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zvv.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bir.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fhv.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jvm.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvg.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gbw.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bor.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wbv.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mmd.zhijiandao.cn

[E06] 替换子串
来源：http://fmm.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zzz.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://tov.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zeb.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://wxt.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rog.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xdk.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qya.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://ons.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://sij.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hcv.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://huq.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fcn.zhengqikj.top

TS:   s.split(",")
来源：http://zxb.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://rzr.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zts.yj20258.top

Ruby: s.split(",");  s.split
来源：http://fgm.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uqm.yfazqb.com

[E08] 数组按分隔符合并
来源：http://knj.dianchejie.cn

Py:   ",".join(items)
来源：http://nxz.yvedp.cn


<!-- 参考信息 -->