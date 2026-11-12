代发 wailian999

Java: list.add(4);
来源：http://puj.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://ifi.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://emm.tarul.cn

C#:   list.Add(4);
来源：http://mif.tanke756.top

[D03] 在指定位置插入元素
来源：http://olr.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://hnv.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rle.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ovw.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://vsq.hnxiangtu.top

Java: list.add(0, 0);
来源：http://imc.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://myj.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://guo.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://syh.zhijiandao.cn

[D04] 删除元素
来源：http://rvs.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tpi.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xgf.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nlw.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://lsm.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mum.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qld.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cws.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ost.mhx1999.top

[D05] 访问与修改元素
来源：http://nel.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ufg.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jot.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ukd.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://sqf.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://vfx.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wux.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ohi.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxg.dianchejie.cn

[D06] 数组长度
来源：http://ncb.yongpay.top

Py:   len(arr)
来源：http://waw.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://gbp.feifeiyinyue.top

JS:   arr.length
来源：http://kxl.zdqjudy.top

TS:   arr.length
来源：http://flw.uphjek.com

Java: list.size();
来源：http://sgo.bbcook.cn

Go:   len(arr)
来源：http://hje.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://whx.jinqigfzy.top

C#:   list.Count;
来源：http://qgr.xziqi.cn

[D07] 切片 / 取子数组
来源：http://hds.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vhy.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qpf.cashguo.top

JS:   arr.slice(1, 4);
来源：http://ywp.uphjek.com

TS:   arr.slice(1, 4);
来源：http://nhb.sxryk.cn

Java: list.subList(1, 4);
来源：http://ryx.zdbjq.cn

Go:   arr[1:4]
来源：http://eno.sufxvd.cn

Ruby: arr[1, 3]
来源：http://chg.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://bhh.dianchejie.cn

[D08] 合并两个数组
来源：http://ayq.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://oog.birdmap.top

PHP:  array_merge($a, $b);
来源：http://hoc.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ykr.zhixingplan.top

TS:   [...a, ...b];
来源：http://fir.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://peo.vehdjk.com

Go:   append(a, b...)
来源：http://wki.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://qhj.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://lad.hnqzz.top

[D09] 排序（升序）
来源：http://irt.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://onp.quarkkingdee.top

PHP:  sort($arr);
来源：http://jxc.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ilh.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bbt.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jkp.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wzt.hammf.cn

Ruby: arr.sort
来源：http://aay.vehdjk.com

C#:   list.Sort();
来源：http://ilt.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gml.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iox.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://clk.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ukh.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgi.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pdr.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cla.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mue.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sni.chenlongwang.top

[D11] 反转数组
来源：http://fxg.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tsk.316326.xyz

PHP:  array_reverse($arr);
来源：http://asf.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uaq.tian-w.cn

TS:   [...arr].reverse();
来源：http://ojx.gzhubu.top

Java: Collections.reverse(list);
来源：http://foj.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://ksg.hcnkem.com

Ruby: arr.reverse
来源：http://sac.uphjek.com

C#:   list.Reverse();
来源：http://uxj.hnqzz.top

[D12] 查找元素下标
来源：http://hck.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://kid.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mou.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kww.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zyw.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpf.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://dtg.uphjek.com

Ruby: arr.index(x)
来源：http://eqz.zycfv.cn

C#:   list.IndexOf(x);
来源：http://yxb.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://jmz.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wsk.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hri.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://cee.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://hnc.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jwr.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ehf.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lpg.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://abe.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://uev.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tdz.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://alt.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://gug.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://yka.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ukj.tarul.cn

Go:   // 手写循环
来源：http://zac.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zyb.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://foi.yuxming.cn

[D15] 去重
来源：http://sur.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jit.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://pxz.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://vny.yuxming.cn

TS:   [...new Set(arr)]
来源：http://cvh.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sym.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://oqz.pycfn.com

Ruby: arr.uniq
来源：http://xdr.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://qig.9152youxi.cn

[D16] 求和与平均值
来源：http://kcy.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cqe.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ndd.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rum.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnb.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://omj.tanke756.top

Go:   // 手写循环累加
来源：http://zxe.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xry.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://hci.gogol.net.cn

[D17] 最大值与最小值
来源：http://psg.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://bzj.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://pdy.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nna.52xcode.cn

TS:   Math.max(...arr);
来源：http://tpm.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zra.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dav.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://gls.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://vpb.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://mnh.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zve.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://qmc.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tmp.haohaochexian.top

TS:   nested.flat();
来源：http://zts.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gbv.aizwys.cn

Go:   // 手写双层循环
来源：http://scz.nwbrower.top

Ruby: nested.flatten
来源：http://bbu.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://omh.shangyingyoupin.top

[D19] 按字段分组
来源：http://yhi.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ajx.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ype.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://orx.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ihj.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vwf.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://xxc.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rxh.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsf.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://fdr.cashguo.top

Py:   Counter(arr)
来源：http://pdy.yj20258888.top

PHP:  array_count_values($arr);
来源：http://kuo.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lfo.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://apy.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tdt.daria6918.cn

Go:   // 手写 map[T]int
来源：http://brs.hnqzz.top

Ruby: arr.tally
来源：http://ffc.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zdr.daria6918.cn

[D21] 判断是否包含某元素
来源：http://cpl.cqqwz.cn

Py:   x in arr
来源：http://nzy.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://hgc.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://cev.yuanzhike.top

TS:   arr.includes(x)
来源：http://ojs.zhengqikj.top

Java: list.contains(x)
来源：http://cus.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://lyq.wangdashe.top

Ruby: arr.include?(x)
来源：http://lsj.ybcxt.top

C#:   list.Contains(x)
来源：http://nfo.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xhn.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://def.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jgw.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mid.smart0.xyz

TS:   [...arr];
来源：http://cpi.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://cnh.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://tpu.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://pfk.kuanghao11.cn

C#:   new List<int>(list);
来源：http://dxj.hywenlv.cn

[D23] reduce 累积计算
来源：http://fqx.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qwx.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mfi.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njh.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qln.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xod.xinyue.icu

Go:   // 手写循环
来源：http://sct.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nbr.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rka.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://oox.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dfw.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvu.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lil.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ryo.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://umf.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sag.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qxx.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gta.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://rjq.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bfc.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pvo.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wka.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://scn.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whj.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://egh.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ise.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nwq.smart0.xyz

[D26] 数组转字符串
来源：http://bgi.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://pzc.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://uid.dianchejie.cn

JS:   arr.join(", ")
来源：http://jwj.sufxvd.cn

TS:   arr.join(", ")
来源：http://vgh.zhongyouzk.top

Java: String.join(", ", list)
来源：http://kkz.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://jvc.redwolf501.top

Ruby: arr.join(", ")
来源：http://wss.fktsv.cn

C#:   string.Join(", ", list)
来源：http://frq.yuanzhike.top

================================================================================
来源：http://kad.cheryme.top

E. 字符串处理
来源：http://wod.jinghuilouyu.cn

================================================================================
来源：http://hwg.daxiang520.top

[E01] 拼接字符串
来源：http://gpy.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gze.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uch.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xvl.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mjv.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wzl.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://urf.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sjg.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hje.sweek.top

[E02] 重复字符串
来源：http://tqp.yj20258888.top

Py:   "ab" * 3
来源：http://ine.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://eps.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://cqu.cucudq.cn

TS:   "ab".repeat(3)
来源：http://qur.fzhhl.top

Java: "ab".repeat(3)
来源：http://iar.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://wwn.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://vkt.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://doo.316326.xyz

[E03] 截取子串
来源：http://lat.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mjk.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qbs.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yvs.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://udo.mhx1999.top

Java: s.substring(1, 4)
来源：http://mfu.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hle.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://csd.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://szh.hnqzz.top

[E04] 查找子串位置
来源：http://nix.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://fsh.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://dxm.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kap.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://xvp.vqdsnc.cn

Java: s.indexOf("x")
来源：http://djs.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://dja.nwbrower.top

Ruby: s.index("x")
来源：http://ykw.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://hcv.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://llk.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iau.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jtt.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xsn.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ajn.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gij.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pqn.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qmz.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kiq.yangfankeji.com

[E06] 替换子串
来源：http://ytr.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wmp.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://thm.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yat.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://ilv.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufi.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bap.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kby.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://xhs.epnwcf.com

[E07] 按分隔符拆分
来源：http://xul.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sav.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hbm.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hjb.fzhhl.top

TS:   s.split(",")
来源：http://rix.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://cbo.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wag.pycfn.com

Ruby: s.split(",");  s.split
来源：http://fzr.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gdl.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://kat.redwolf501.top

Py:   ",".join(items)
来源：http://hfy.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://ayu.52xcode.cn

JS:   items.join(",")
来源：http://rno.cucudq.cn

TS:   items.join(",")
来源：http://fec.guowangkeji.top

Java: String.join(",", items)
来源：http://fbv.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://nkn.fzhhl.top

Ruby: items.join(",")
来源：http://nyo.gotoacloud.top

C#:   string.Join(",", items)
来源：http://rjy.guowangkeji.top

[E09] 去除所有空白字符
来源：http://znt.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://llf.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xyl.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://yfj.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://cwr.shanyushiyangkeji.top


<!-- 参考信息 -->