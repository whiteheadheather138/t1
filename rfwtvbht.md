代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://nfq.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://ihs.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rtd.gzhubu.top

[D02] 追加元素到末尾
来源：http://smi.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ypq.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://syf.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://ead.tanke756.top

TS:   arr.push(4);
来源：http://mhv.redwolf501.top

Java: list.add(4);
来源：http://lyn.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://lyp.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://jhd.hammf.cn

C#:   list.Add(4);
来源：http://iwj.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://lvb.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://shk.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xvv.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://suk.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://uqi.ydzc1.top

Java: list.add(0, 0);
来源：http://gbq.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jsx.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hqm.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://sxo.xziqi.cn

[D04] 删除元素
来源：http://qqa.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xyb.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gxe.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sce.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://dso.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xos.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qnf.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gle.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://frn.bbcook.cn

[D05] 访问与修改元素
来源：http://ywp.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nmi.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://spd.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wrp.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://kgk.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://skc.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://vlw.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ndo.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pna.birdmap.top

[D06] 数组长度
来源：http://zmr.meibo888.top

Py:   len(arr)
来源：http://pio.svipenyu.cn

PHP:  count($arr);
来源：http://deu.tianlin.xyz

JS:   arr.length
来源：http://uoy.shanyushiyangkeji.top

TS:   arr.length
来源：http://evh.xylfe.cn

Java: list.size();
来源：http://sgy.nanxinkj.top

Go:   len(arr)
来源：http://cvx.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://xmu.yongpay.top

C#:   list.Count;
来源：http://ruc.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://mgw.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pfd.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://zfh.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://drf.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://uqq.yuxming.cn

Java: list.subList(1, 4);
来源：http://yvl.epnwcf.com

Go:   arr[1:4]
来源：http://ban.ydzc1.top

Ruby: arr[1, 3]
来源：http://plq.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://ycm.zhengqikj.top

[D08] 合并两个数组
来源：http://oxe.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://tvh.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://ngk.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://rzj.gzhubu.top

TS:   [...a, ...b];
来源：http://gti.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxz.sweek.top

Go:   append(a, b...)
来源：http://cvz.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://xqz.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://vxj.jqgfzy.top

[D09] 排序（升序）
来源：http://bol.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://ybw.yongpay.top

PHP:  sort($arr);
来源：http://hsu.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vua.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://opy.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bli.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kii.haohaochexian.top

Ruby: arr.sort
来源：http://sgl.fktsv.cn

C#:   list.Sort();
来源：http://vph.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gad.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpw.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tfz.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://udl.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fco.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fkg.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://udj.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yhp.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wmu.shanyushiyangtech.top

[D11] 反转数组
来源：http://woh.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kqa.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://mar.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rto.zhixingplan.top

TS:   [...arr].reverse();
来源：http://ouq.iojbl.cn

Java: Collections.reverse(list);
来源：http://iyn.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://nts.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://klp.hcnkem.com

C#:   list.Reverse();
来源：http://wlh.aibaodan.cn

[D12] 查找元素下标
来源：http://yux.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://kvn.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ybo.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vxf.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vnk.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vbs.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://dxu.hcnkem.com

Ruby: arr.index(x)
来源：http://sxg.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://ynr.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://jxk.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yih.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gkx.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://wlz.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://als.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dvg.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dqq.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://mjh.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://und.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://lgl.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rfj.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zbh.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://eql.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://xli.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://cdq.nanxinkj.top

Go:   // 手写循环
来源：http://noe.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tyz.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://wje.pengpengdd.cyou

[D15] 去重
来源：http://sjg.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qze.cashguo.top

PHP:  array_unique($arr);
来源：http://wtc.xziqi.cn

JS:   [...new Set(arr)]
来源：http://nsy.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://hzp.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iav.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://htp.yfazqb.com

Ruby: arr.uniq
来源：http://ikx.tanke756.top

C#:   list.Distinct().ToList()
来源：http://nto.cucudq.cn

[D16] 求和与平均值
来源：http://odt.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://txv.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tss.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqa.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bti.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gff.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://rfy.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uca.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://wmq.hysaishi.cn

[D17] 最大值与最小值
来源：http://qkp.hammf.cn

Py:   max(arr);  min(arr)
来源：http://rqm.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://btr.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hur.pycfn.com

TS:   Math.max(...arr);
来源：http://pih.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zrt.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vqm.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://vqn.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://eke.yonumen.top

[D18] 扁平化嵌套数组
来源：http://sjs.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rey.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://ovl.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qkd.fehbvm.com

TS:   nested.flat();
来源：http://jfb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cal.smart0.xyz

Go:   // 手写双层循环
来源：http://cng.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://vts.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ids.redwolf501.top

[D19] 按字段分组
来源：http://wnt.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ept.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nad.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zmb.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://roa.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://piy.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://wsq.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xuy.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://agv.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ebb.bbcook.cn

Py:   Counter(arr)
来源：http://cnb.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://xwy.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oim.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mhw.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oav.yonumen.top

Go:   // 手写 map[T]int
来源：http://sob.zhixingplan.top

Ruby: arr.tally
来源：http://lej.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vzc.ydzc1.top

[D21] 判断是否包含某元素
来源：http://wak.chenlongwang.top

Py:   x in arr
来源：http://mkp.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://vwj.birdmap.top

JS:   arr.includes(x)
来源：http://ivu.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://aie.smart0.xyz

Java: list.contains(x)
来源：http://plu.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://bdv.shzxlz.cn

Ruby: arr.include?(x)
来源：http://ctw.yuanzhike.top

C#:   list.Contains(x)
来源：http://xrt.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://fyt.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qxp.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://upq.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hkk.nanxuanxn.top

TS:   [...arr];
来源：http://fvl.yonumen.top

Java: new ArrayList<>(list);
来源：http://rcl.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://mpb.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://tlx.yanxiufei.cn

C#:   new List<int>(list);
来源：http://ceh.ctjpmb.com

[D23] reduce 累积计算
来源：http://klw.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ywp.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kiu.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wfh.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsq.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://wkk.chenzaomai.com

Go:   // 手写循环
来源：http://qyp.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mvu.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zia.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://dbz.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwe.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qkz.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vnb.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xth.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lek.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aix.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fcd.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cwy.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://emp.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eey.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wdb.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xxx.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://une.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fqd.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sgb.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://clg.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vyf.birdmap.top

[D26] 数组转字符串
来源：http://ian.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://hhz.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://mdt.0kj1m.cn

JS:   arr.join(", ")
来源：http://iou.bbcook.cn

TS:   arr.join(", ")
来源：http://rnj.sjlbkw.cn

Java: String.join(", ", list)
来源：http://uvs.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://arg.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://obp.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://vps.snrcjt.cn

================================================================================
来源：http://jsf.guowangkeji.top

E. 字符串处理
来源：http://bmd.fzhhl.top

================================================================================
来源：http://tzj.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://yqa.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gtb.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qsd.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kol.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aaw.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hww.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oxr.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://edd.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rrr.ydzc1.top

[E02] 重复字符串
来源：http://ulq.zhengqikj.top

Py:   "ab" * 3
来源：http://nft.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://itl.xuanzx.com

JS:   "ab".repeat(3)
来源：http://ojx.mhx1999.top

TS:   "ab".repeat(3)
来源：http://lpz.hywenlv.cn

Java: "ab".repeat(3)
来源：http://sct.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://cif.aizwys.cn

Ruby: "ab" * 3
来源：http://oao.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qke.vqdsnc.cn

[E03] 截取子串
来源：http://jtd.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wkc.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxl.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xfx.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://qzc.smart0.xyz

Java: s.substring(1, 4)
来源：http://aip.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tby.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://vsd.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://hxk.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://ecd.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://bfe.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://nqo.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vge.snrcjt.cn

TS:   s.indexOf("x")
来源：http://lkv.jqgufenzy.top

Java: s.indexOf("x")
来源：http://pnq.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://oiw.yvedp.cn

Ruby: s.index("x")
来源：http://ulv.uphjek.com

C#:   s.IndexOf("x")
来源：http://win.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zom.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ztz.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mkm.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mba.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://itu.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tir.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://abo.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ota.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pic.dashuyun.cn

[E06] 替换子串
来源：http://vtc.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lkf.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://cvm.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ukf.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://tia.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mgk.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nio.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hxu.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://ror.zdqjudy.top

[E07] 按分隔符拆分
来源：http://mmp.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wfh.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zcm.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rpt.hfpthk.cn

TS:   s.split(",")
来源：http://krh.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qvl.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxk.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://asp.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ump.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://etv.aibaodan.cn

Py:   ",".join(items)
来源：http://heu.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://ccr.shuidangran.top

JS:   items.join(",")
来源：http://ope.bjfxy.top

TS:   items.join(",")
来源：http://rtv.hfpthk.cn

Java: String.join(",", items)
来源：http://xsv.birdmap.top


<!-- 参考信息 -->