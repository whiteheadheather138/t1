代发 wailian999

D. 数组 / 列表 / 集合
来源：http://spd.hongshengwenyu.top

================================================================================
来源：http://sab.ivvv.top

[D01] 创建数组 / 列表
来源：http://hjz.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://yzq.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xto.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uss.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://glm.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rqv.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://ben.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://rhr.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vpk.tianlin.xyz

[D02] 追加元素到末尾
来源：http://ssn.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rol.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uue.aizwys.cn

JS:   arr.push(4);
来源：http://abp.zhengqikj.top

TS:   arr.push(4);
来源：http://vjz.hcnkem.com

Java: list.add(4);
来源：http://tlq.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://nwo.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://dhb.hcnkem.com

C#:   list.Add(4);
来源：http://emh.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://yvr.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://igk.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iip.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sie.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://kzu.sysykeji.top

Java: list.add(0, 0);
来源：http://xit.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://clq.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qrh.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://nvk.havefunace.top

[D04] 删除元素
来源：http://ouc.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://buh.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dip.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rix.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://hqw.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qaw.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipk.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tbu.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nbm.jqgfzy.top

[D05] 访问与修改元素
来源：http://ufa.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lir.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nfo.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://prh.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://dtq.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://icr.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://bmh.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bin.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yoc.jinghuilouyu.cn

[D06] 数组长度
来源：http://jra.yongpay.top

Py:   len(arr)
来源：http://smy.yj20258888.top

PHP:  count($arr);
来源：http://ddf.shanyushiyangtech.top

JS:   arr.length
来源：http://tde.hesvh.cn

TS:   arr.length
来源：http://eiy.yfazqb.com

Java: list.size();
来源：http://bbw.jyoumei.cn

Go:   len(arr)
来源：http://icr.gzhubu.top

Ruby: arr.length; arr.size
来源：http://nqg.bjfxy.top

C#:   list.Count;
来源：http://fek.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://ekp.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qjf.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kbt.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://wcf.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://fsg.xziqi.cn

Java: list.subList(1, 4);
来源：http://hif.cdnleiting.top

Go:   arr[1:4]
来源：http://anc.sufxvd.cn

Ruby: arr[1, 3]
来源：http://yez.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://tvv.yvedp.cn

[D08] 合并两个数组
来源：http://plu.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://caj.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://ctj.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kmu.vqdsnc.cn

TS:   [...a, ...b];
来源：http://mkw.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uvu.yj202588.top

Go:   append(a, b...)
来源：http://xpt.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://sja.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://yjb.haohaochexian.top

[D09] 排序（升序）
来源：http://hko.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://qtr.meibo888.top

PHP:  sort($arr);
来源：http://iiw.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dwc.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iou.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://djt.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mdt.kuanghao11.cn

Ruby: arr.sort
来源：http://czn.feifeiyinyue.top

C#:   list.Sort();
来源：http://pmn.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dqu.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvv.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofr.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uaj.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjc.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://upp.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pqg.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ltf.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mod.vehdjk.com

[D11] 反转数组
来源：http://xek.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://dnp.fengsongda.top

PHP:  array_reverse($arr);
来源：http://mpm.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ujf.yuanzhike.top

TS:   [...arr].reverse();
来源：http://mna.meibo888.top

Java: Collections.reverse(list);
来源：http://yek.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://bun.zycfv.cn

Ruby: arr.reverse
来源：http://urv.yangfankeji.com

C#:   list.Reverse();
来源：http://ltk.pengpengdd.cyou

[D12] 查找元素下标
来源：http://brj.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://yed.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sfx.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://amk.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esw.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://drj.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://eje.fengsongda.top

Ruby: arr.index(x)
来源：http://jfc.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://qzk.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://lis.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dwo.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rlj.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://nxj.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://opf.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dea.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://shb.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://wxo.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://slj.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://cpi.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iyg.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kte.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://czd.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://kyx.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://srl.hcnkem.com

Go:   // 手写循环
来源：http://vra.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://gyy.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lae.hesvh.cn

[D15] 去重
来源：http://kbl.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rpz.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://zcw.uphjek.com

JS:   [...new Set(arr)]
来源：http://vlb.vehdjk.com

TS:   [...new Set(arr)]
来源：http://zgu.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lnw.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://nbv.iojbl.cn

Ruby: arr.uniq
来源：http://sqa.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://pmv.fengsongda.top

[D16] 求和与平均值
来源：http://lmu.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wbj.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pnp.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wwz.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ipx.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tuw.yueranfly.top

Go:   // 手写循环累加
来源：http://vqz.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uws.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://pbs.zhijiandao.cn

[D17] 最大值与最小值
来源：http://aot.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://ekr.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://vub.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oso.ehwqpu.com

TS:   Math.max(...arr);
来源：http://drb.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wiw.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jgd.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://uum.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://etu.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://jyw.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nfs.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://pzz.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bdb.shanyushiyangtech.top

TS:   nested.flat();
来源：http://uhk.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kxz.sysykeji.top

Go:   // 手写双层循环
来源：http://jbc.fzhhl.top

Ruby: nested.flatten
来源：http://agb.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://asr.ppjwa.cn

[D19] 按字段分组
来源：http://nbc.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tkr.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qun.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wdg.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://suy.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aty.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://hvw.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qlu.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nvs.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://rdi.nanxuanxn.top

Py:   Counter(arr)
来源：http://bpy.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://mqj.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bet.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://juq.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qlc.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://zdn.zhiwuduotai.top

Ruby: arr.tally
来源：http://qnb.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwy.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://ntw.hnxiangtu.top

Py:   x in arr
来源：http://fwy.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://kuc.jqgufenzy.top

JS:   arr.includes(x)
来源：http://tqr.yvedp.cn

TS:   arr.includes(x)
来源：http://udy.shangyingyoupin.top

Java: list.contains(x)
来源：http://bax.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://suv.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://qoy.jianghu66.top

C#:   list.Contains(x)
来源：http://kve.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://clm.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iuc.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nwb.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fjc.hnxiangtu.top

TS:   [...arr];
来源：http://aen.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://vgw.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://zcn.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://ddo.bjfxy.top

C#:   new List<int>(list);
来源：http://jhk.vehdjk.com

[D23] reduce 累积计算
来源：http://jyp.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://trr.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pkx.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vud.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ely.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://plc.gaohongyu789.top

Go:   // 手写循环
来源：http://adk.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jlf.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ltq.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://rbo.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ycb.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://exu.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bjw.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xeq.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hgs.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pvr.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hjq.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rmu.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://uap.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xzx.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ibj.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bak.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pcg.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ibf.yj20258888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kfs.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jsi.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://smj.xylfe.cn

[D26] 数组转字符串
来源：http://sqo.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://rla.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://jns.yj20258888.top

JS:   arr.join(", ")
来源：http://aif.cheryme.top

TS:   arr.join(", ")
来源：http://jhm.birdmap.top

Java: String.join(", ", list)
来源：http://rhl.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://eun.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://hdz.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://rnl.jianghu66.top

================================================================================
来源：http://xvv.smart0.xyz

E. 字符串处理
来源：http://clq.wangdashe.top

================================================================================
来源：http://idv.xylfe.cn

[E01] 拼接字符串
来源：http://ppv.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://arz.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysh.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxg.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eyk.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zwb.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iim.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vsp.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hle.gogol.net.cn

[E02] 重复字符串
来源：http://kft.ydzc1.top

Py:   "ab" * 3
来源：http://sdb.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://ocw.bjfxy.top

JS:   "ab".repeat(3)
来源：http://lsc.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://oag.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://qtf.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://znr.ybcxt.top

Ruby: "ab" * 3
来源：http://pay.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bvg.zhoulong.xyz

[E03] 截取子串
来源：http://jyh.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ufc.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ldr.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gtp.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://prg.yuxming.cn

Java: s.substring(1, 4)
来源：http://dci.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pzy.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://lss.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://enx.xylfe.cn

[E04] 查找子串位置
来源：http://cbd.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://umy.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://zfw.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wti.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://ong.cdnleiting.top

Java: s.indexOf("x")
来源：http://sci.yonumen.top

Go:   strings.Index(s, "x")
来源：http://xbr.jiagoushi.top

Ruby: s.index("x")
来源：http://xnj.sweek.top

C#:   s.IndexOf("x")
来源：http://nsa.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://fry.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqa.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xvb.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhy.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpy.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dkz.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vco.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dem.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jug.yonumen.top

[E06] 替换子串
来源：http://uhv.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzk.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://ksl.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omr.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://pkn.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvm.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ujt.ivvv.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cmi.tarul.cn

C#:   s.Replace("a", "b")
来源：http://dik.yj20258888.top

[E07] 按分隔符拆分
来源：http://trm.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fyx.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sfg.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yur.daria6918.cn

TS:   s.split(",")
来源：http://bkd.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://yeu.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iiq.ywan-chungtsiang.top


<!-- 参考信息 -->