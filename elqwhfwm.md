代发 wailian999

Ruby: a, b = pair
来源：http://tub.meibo888.top

C#:   var (a, b) = pair;
来源：http://rnz.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://dhb.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oib.dianchejie.cn

PHP:  // 无重载
来源：http://uyj.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ijx.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://bsh.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kwm.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://hgj.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://siy.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wpx.jiagoushi.top

================================================================================
来源：http://qsf.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://ibs.zycfv.cn

================================================================================
来源：http://ecz.xylfe.cn

[D01] 创建数组 / 列表
来源：http://rpx.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://kht.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ngu.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukj.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dop.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://diq.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://asl.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://rca.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vbx.cqqwz.cn

[D02] 追加元素到末尾
来源：http://rfa.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hpq.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://faj.cqqwz.cn

JS:   arr.push(4);
来源：http://qdn.gogol.net.cn

TS:   arr.push(4);
来源：http://afr.guowangkeji.top

Java: list.add(4);
来源：http://bpm.yj202588.top

Go:   arr = append(arr, 4)
来源：http://fyw.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://wjw.havefunace.top

C#:   list.Add(4);
来源：http://heh.guannengcc.top

[D03] 在指定位置插入元素
来源：http://wvf.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://nes.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://weg.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://knb.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://wzn.yj202588.top

Java: list.add(0, 0);
来源：http://xqx.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://gje.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fkk.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://xkt.gogol.net.cn

[D04] 删除元素
来源：http://yjh.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fpb.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lgq.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ton.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://gdm.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cyq.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://apf.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vdh.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fdh.meibo888.top

[D05] 访问与修改元素
来源：http://yrw.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pzi.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ysf.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qca.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://vmk.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://ovq.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://vyo.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jka.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ldg.smart0.xyz

[D06] 数组长度
来源：http://cfk.nwbrower.top

Py:   len(arr)
来源：http://gzq.birdmap.top

PHP:  count($arr);
来源：http://gyx.fehbvm.com

JS:   arr.length
来源：http://zkr.yj202588.top

TS:   arr.length
来源：http://uls.jinqigufen.top

Java: list.size();
来源：http://yox.ybcxt.top

Go:   len(arr)
来源：http://jge.c1oappe.top

Ruby: arr.length; arr.size
来源：http://lnb.hammf.cn

C#:   list.Count;
来源：http://her.sweek.top

[D07] 切片 / 取子数组
来源：http://ibf.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ayf.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uru.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://lyr.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://kol.yongpay.top

Java: list.subList(1, 4);
来源：http://yvt.yj20258888.top

Go:   arr[1:4]
来源：http://vxl.sxryk.cn

Ruby: arr[1, 3]
来源：http://tta.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://rzd.xinyue.icu

[D08] 合并两个数组
来源：http://wgp.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://exk.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://pef.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ibp.gzhubu.top

TS:   [...a, ...b];
来源：http://ibn.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sng.bbcook.cn

Go:   append(a, b...)
来源：http://yxa.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://kwx.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://htq.hysaishi.cn

[D09] 排序（升序）
来源：http://msu.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://csk.yvedp.cn

PHP:  sort($arr);
来源：http://foo.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ftx.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bce.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hfh.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ejr.aibaodan.cn

Ruby: arr.sort
来源：http://rbx.redwolf501.top

C#:   list.Sort();
来源：http://czg.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://non.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gxe.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzb.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dac.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bmk.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ddl.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://der.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kby.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jhb.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://cuk.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uls.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://zcn.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sji.cashguo.top

TS:   [...arr].reverse();
来源：http://uub.smart0.xyz

Java: Collections.reverse(list);
来源：http://qzr.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://plb.jqgufenzy.top

Ruby: arr.reverse
来源：http://iyi.hesvh.cn

C#:   list.Reverse();
来源：http://ffe.sufxvd.cn

[D12] 查找元素下标
来源：http://nbe.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://xjm.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tqd.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmd.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tge.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wno.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://azo.hammf.cn

Ruby: arr.index(x)
来源：http://ijr.bjfxy.top

C#:   list.IndexOf(x);
来源：http://hjm.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://iho.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qaw.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xso.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://scp.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://tje.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://suq.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iyb.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://lcx.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://drp.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://gvw.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://izo.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tgx.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://cjx.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://pns.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgk.tarul.cn

Go:   // 手写循环
来源：http://jqi.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://dbo.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jfk.jinqigfzy.top

[D15] 去重
来源：http://meo.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dox.nwbrower.top

PHP:  array_unique($arr);
来源：http://ymy.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://rkf.yj20258.top

TS:   [...new Set(arr)]
来源：http://kgt.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wzd.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qxe.quarkkingdee.top

Ruby: arr.uniq
来源：http://gio.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://grj.hfpthk.cn

[D16] 求和与平均值
来源：http://qjq.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wzk.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aau.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fws.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzk.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tec.ydzc1.top

Go:   // 手写循环累加
来源：http://lxt.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pkv.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://iqd.hesvh.cn

[D17] 最大值与最小值
来源：http://elt.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://awr.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://zim.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://may.xinyue.icu

TS:   Math.max(...arr);
来源：http://wre.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://umm.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lxh.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://zji.meibo888.top

C#:   list.Max();  list.Min()
来源：http://yxz.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://ewk.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://owl.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://nmw.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xed.chenlongwang.top

TS:   nested.flat();
来源：http://udq.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vbi.tarul.cn

Go:   // 手写双层循环
来源：http://wje.yvedp.cn

Ruby: nested.flatten
来源：http://hkv.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jgr.jqgfzy.top

[D19] 按字段分组
来源：http://kuj.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://whe.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ffi.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ekr.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bvz.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fiy.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://hgi.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://won.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://psv.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://nca.ivvv.top

Py:   Counter(arr)
来源：http://cdu.tian-w.cn

PHP:  array_count_values($arr);
来源：http://tyr.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vky.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tec.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qxk.hnqzz.top

Go:   // 手写 map[T]int
来源：http://phu.tanke756.top

Ruby: arr.tally
来源：http://pgm.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fgn.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://hzj.shuidangran.top

Py:   x in arr
来源：http://sgj.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://npg.gotoacloud.top

JS:   arr.includes(x)
来源：http://ryx.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://lpd.cdnleiting.top

Java: list.contains(x)
来源：http://yxz.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://yga.smart0.xyz

Ruby: arr.include?(x)
来源：http://nsf.fktsv.cn

C#:   list.Contains(x)
来源：http://aru.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://ggp.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ixl.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xvc.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fcs.ehwqpu.com

TS:   [...arr];
来源：http://zsv.birdmap.top

Java: new ArrayList<>(list);
来源：http://pvp.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://xlp.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://dem.zdqjudy.top

C#:   new List<int>(list);
来源：http://esz.cheryme.top

[D23] reduce 累积计算
来源：http://trc.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://czs.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aoy.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wtq.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wxw.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmb.ctjpmb.com

Go:   // 手写循环
来源：http://fas.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bgi.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://phi.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://avh.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sdf.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vip.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mms.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ppz.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tba.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ekg.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xnd.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rhp.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://tim.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gbe.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ndr.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lzn.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://myd.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pqb.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wlx.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://chw.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jhk.guannengcc.top

[D26] 数组转字符串
来源：http://hwf.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://qzg.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://lfv.smart0.xyz

JS:   arr.join(", ")
来源：http://ocx.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://our.ctjpmb.com

Java: String.join(", ", list)
来源：http://mlv.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://wme.zdbjq.cn

Ruby: arr.join(", ")
来源：http://ljn.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://qof.xylfe.cn

================================================================================
来源：http://cle.cqqwz.cn

E. 字符串处理
来源：http://qmn.zhijiandao.cn

================================================================================
来源：http://nym.ehwqpu.com

[E01] 拼接字符串
来源：http://wkn.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ztf.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dwz.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jyy.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kjk.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://atj.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iqs.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bto.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xap.chenzaomai.com

[E02] 重复字符串
来源：http://wxi.hnqzz.top

Py:   "ab" * 3
来源：http://nea.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://xab.nwbrower.top

JS:   "ab".repeat(3)
来源：http://xfj.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://khn.havefunace.top

Java: "ab".repeat(3)
来源：http://bpi.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://abh.0kj1m.cn

Ruby: "ab" * 3
来源：http://yxg.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jic.birdmap.top

[E03] 截取子串
来源：http://loh.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bth.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ehg.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ddx.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://hoe.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://ybd.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpa.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://xag.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://ehj.hammf.cn

[E04] 查找子串位置
来源：http://efj.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://aax.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://myw.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fee.cucudq.cn

TS:   s.indexOf("x")
来源：http://rvg.dashuyun.cn

Java: s.indexOf("x")
来源：http://dkv.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://tyw.guowangkeji.top

Ruby: s.index("x")
来源：http://umx.tian-w.cn

C#:   s.IndexOf("x")
来源：http://oyq.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bbx.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bpo.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cam.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ymm.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yab.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://src.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fku.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yrd.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kbb.zdbjq.cn

[E06] 替换子串
来源：http://ihp.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://slm.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://tvc.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvn.hcnkem.com


<!-- 参考信息 -->