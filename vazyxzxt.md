代发 wailian999

PHP:  // 无重载
来源：http://evs.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yht.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://cma.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://erz.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://myw.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://lpd.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jwr.pengpengdd.cyou

================================================================================
来源：http://rlc.cashguo.top

D. 数组 / 列表 / 集合
来源：http://nwv.hongshengwenyu.top

================================================================================
来源：http://onj.sweek.top

[D01] 创建数组 / 列表
来源：http://mpr.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://syc.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rdp.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sku.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbp.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mbq.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://psy.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ajg.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xxl.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://zjm.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rdw.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mro.tian-w.cn

JS:   arr.push(4);
来源：http://bso.zhijiandao.cn

TS:   arr.push(4);
来源：http://wgi.shanyushiyangtech.top

Java: list.add(4);
来源：http://ywu.316326.xyz

Go:   arr = append(arr, 4)
来源：http://rcb.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://uhc.aizwys.cn

C#:   list.Add(4);
来源：http://fps.tarul.cn

[D03] 在指定位置插入元素
来源：http://exe.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://dbh.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rey.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nqa.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://nch.redwolf501.top

Java: list.add(0, 0);
来源：http://ahf.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://etw.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bmc.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://tbp.cqqwz.cn

[D04] 删除元素
来源：http://zmc.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zmb.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bfj.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zzx.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://ccu.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://khw.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mqp.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jnx.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yve.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://pro.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ewn.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kwd.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://air.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://tld.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://kjq.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://tlj.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://srm.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eyb.xuanzx.com

[D06] 数组长度
来源：http://wcp.tianlin.xyz

Py:   len(arr)
来源：http://gtk.andypj.xyz

PHP:  count($arr);
来源：http://tiy.xingfuxueyuan.xyz

JS:   arr.length
来源：http://dvv.sysykeji.top

TS:   arr.length
来源：http://wkr.0kj1m.cn

Java: list.size();
来源：http://aoe.xinyue.icu

Go:   len(arr)
来源：http://mcg.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://dum.dianchejie.cn

C#:   list.Count;
来源：http://bhc.zycfv.cn

[D07] 切片 / 取子数组
来源：http://jgk.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aoh.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jsm.hammf.cn

JS:   arr.slice(1, 4);
来源：http://aqy.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://fxf.ivvv.top

Java: list.subList(1, 4);
来源：http://mrw.cucudq.cn

Go:   arr[1:4]
来源：http://pzo.guannengcc.top

Ruby: arr[1, 3]
来源：http://vah.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://hzx.pycfn.com

[D08] 合并两个数组
来源：http://ipb.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://jss.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://mic.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dwt.gzhubu.top

TS:   [...a, ...b];
来源：http://bxj.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nys.meibo888.top

Go:   append(a, b...)
来源：http://aor.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://hjx.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://qwz.gotoacloud.top

[D09] 排序（升序）
来源：http://nwo.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://trd.gogol.net.cn

PHP:  sort($arr);
来源：http://tdy.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hih.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jzl.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vdb.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fef.yangfankeji.com

Ruby: arr.sort
来源：http://eub.hcnkem.com

C#:   list.Sort();
来源：http://xdm.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://rbt.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pfy.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hcs.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://myo.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgv.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efd.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ivm.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qht.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cqr.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://vte.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ypt.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://luc.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nfl.daxiang520.top

TS:   [...arr].reverse();
来源：http://dfi.9152youxi.cn

Java: Collections.reverse(list);
来源：http://xoc.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://gzm.hnqzz.top

Ruby: arr.reverse
来源：http://row.zhongyouzk.top

C#:   list.Reverse();
来源：http://nnq.bjfxy.top

[D12] 查找元素下标
来源：http://byq.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://muw.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gle.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mqj.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eti.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jys.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://scm.andypj.xyz

Ruby: arr.index(x)
来源：http://tyd.hnqzz.top

C#:   list.IndexOf(x);
来源：http://mnw.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://mwf.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dlc.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ipr.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://vha.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://qzq.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hyb.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wpu.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://voj.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://peo.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://gpt.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ebz.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhg.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://eal.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://ppo.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bae.hammf.cn

Go:   // 手写循环
来源：http://vdg.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://ond.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uwn.shanyushiyangtech.top

[D15] 去重
来源：http://vjy.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xkw.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://emb.xinyue.icu

JS:   [...new Set(arr)]
来源：http://ryp.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://gog.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cpx.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://kzp.uphjek.com

Ruby: arr.uniq
来源：http://lvp.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://fgb.chenlongwang.top

[D16] 求和与平均值
来源：http://nry.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fdg.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yfa.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rwx.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://drp.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yow.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://swe.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dlc.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://cwq.zycfv.cn

[D17] 最大值与最小值
来源：http://mkm.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://qrc.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://jtt.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bdo.hammf.cn

TS:   Math.max(...arr);
来源：http://wal.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://awb.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://njb.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://hds.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://vxo.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://eft.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hxw.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://pcn.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uus.mhx1999.top

TS:   nested.flat();
来源：http://zyd.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xud.snrcjt.cn

Go:   // 手写双层循环
来源：http://ikn.nanxuanxn.top

Ruby: nested.flatten
来源：http://vsq.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xhx.0kj1m.cn

[D19] 按字段分组
来源：http://qsv.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jxu.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ggf.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uaw.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lky.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nul.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://vzl.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ipe.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfi.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://fys.hesvh.cn

Py:   Counter(arr)
来源：http://cbs.birdmap.top

PHP:  array_count_values($arr);
来源：http://zld.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afe.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oqi.tian-w.cn

Go:   // 手写 map[T]int
来源：http://ohc.ivvv.top

Ruby: arr.tally
来源：http://nai.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vkm.cashguo.top

[D21] 判断是否包含某元素
来源：http://rop.cashguo.top

Py:   x in arr
来源：http://ohx.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://buj.sysykeji.top

JS:   arr.includes(x)
来源：http://odr.yangfankeji.com

TS:   arr.includes(x)
来源：http://yvr.chenzaomai.com

Java: list.contains(x)
来源：http://xrm.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://cmq.fktsv.cn

Ruby: arr.include?(x)
来源：http://rlc.jyoumei.cn

C#:   list.Contains(x)
来源：http://nhl.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://sox.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bzv.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uyw.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mus.xinyue.icu

TS:   [...arr];
来源：http://xhl.jianghu66.top

Java: new ArrayList<>(list);
来源：http://qdn.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://yhb.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://blk.hywenlv.cn

C#:   new List<int>(list);
来源：http://rrk.pycfn.com

[D23] reduce 累积计算
来源：http://ykv.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ewz.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dbn.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkb.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chs.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://fyt.fzhhl.top

Go:   // 手写循环
来源：http://qji.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xir.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cgq.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://pqj.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ycn.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsy.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hmk.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ykv.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xaa.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uwk.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ryf.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bpc.yj202588.top

[D25] Set 集合去重与交并差
来源：http://ihp.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fru.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wxy.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://twf.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ctb.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dtf.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xls.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ivb.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://slj.jqgfzy.top

[D26] 数组转字符串
来源：http://zri.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://ahs.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://cow.vqdsnc.cn

JS:   arr.join(", ")
来源：http://urx.ctjpmb.com

TS:   arr.join(", ")
来源：http://vqc.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://idt.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://zfw.xuanzx.com

Ruby: arr.join(", ")
来源：http://sbn.yj20258888.top

C#:   string.Join(", ", list)
来源：http://czz.pycfn.com

================================================================================
来源：http://zuo.hammf.cn

E. 字符串处理
来源：http://sks.yuanzhike.top

================================================================================
来源：http://fat.xinyue.icu

[E01] 拼接字符串
来源：http://nui.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xlj.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kse.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bjm.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gfw.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lcb.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mxg.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://soi.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iot.jinqigufen.top

[E02] 重复字符串
来源：http://uji.shangyingyoupin.top

Py:   "ab" * 3
来源：http://vyr.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://dqx.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://qob.redwolf501.top

TS:   "ab".repeat(3)
来源：http://rvg.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://wkq.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://hoq.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://pqk.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rnz.havefunace.top

[E03] 截取子串
来源：http://shb.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://otx.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wbo.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fmh.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://vxa.0kj1m.cn

Java: s.substring(1, 4)
来源：http://keg.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bkf.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://fzl.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://iaj.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://byc.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://rfv.havefunace.top

PHP:  strpos($s, "x");
来源：http://bop.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qvk.yangfankeji.com

TS:   s.indexOf("x")
来源：http://lex.smart0.xyz

Java: s.indexOf("x")
来源：http://mei.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://jpt.tanke756.top

Ruby: s.index("x")
来源：http://mku.cucudq.cn

C#:   s.IndexOf("x")
来源：http://faa.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xoc.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aku.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fjr.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sei.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mlo.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ifv.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://avl.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pgx.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://anx.zhixingplan.top

[E06] 替换子串
来源：http://hsy.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ucj.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://trw.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nfb.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://ujq.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwg.yuxming.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sqc.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mih.birdmap.top


<!-- 参考信息 -->