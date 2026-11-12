代发 wailian999

Java: list.add(4);
来源：http://urk.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://dbd.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ags.gzhubu.top

C#:   list.Add(4);
来源：http://jkh.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://ngr.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://klg.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gnl.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nkm.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://obm.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://ujh.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://glo.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xgl.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://ppr.jinyuanbaomall.cn

[D04] 删除元素
来源：http://gpc.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mrc.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xoa.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bed.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://awo.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mmd.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rxn.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tgt.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xrd.wangdashe.top

[D05] 访问与修改元素
来源：http://oip.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gfr.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zmb.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kch.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://phm.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://mlv.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://pdw.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://osn.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fxd.aibaodan.cn

[D06] 数组长度
来源：http://fuk.hysaishi.cn

Py:   len(arr)
来源：http://jrg.tian-w.cn

PHP:  count($arr);
来源：http://dhg.yangfankeji.com

JS:   arr.length
来源：http://hun.fehbvm.com

TS:   arr.length
来源：http://kto.wangshuangyany.cn

Java: list.size();
来源：http://nbo.cqqwz.cn

Go:   len(arr)
来源：http://yin.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://lxe.guannengcc.top

C#:   list.Count;
来源：http://ilt.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://agl.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://utf.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://ooy.birdmap.top

JS:   arr.slice(1, 4);
来源：http://tsz.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://kli.316326.xyz

Java: list.subList(1, 4);
来源：http://cyk.yongpay.top

Go:   arr[1:4]
来源：http://kcc.zhengqikj.top

Ruby: arr[1, 3]
来源：http://kyf.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://lul.c1oappe.top

[D08] 合并两个数组
来源：http://kyo.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://dnw.meibo888.top

PHP:  array_merge($a, $b);
来源：http://bsj.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hqi.nanxinkj.top

TS:   [...a, ...b];
来源：http://kyw.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://avz.hysaishi.cn

Go:   append(a, b...)
来源：http://hxc.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://hji.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://qvv.jinqigufen.top

[D09] 排序（升序）
来源：http://bcm.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://pde.cdnleiting.top

PHP:  sort($arr);
来源：http://ios.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fom.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gqc.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbz.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://txi.feifeiyinyue.top

Ruby: arr.sort
来源：http://cjp.redwolf501.top

C#:   list.Sort();
来源：http://zze.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://deg.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://par.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vxz.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hvl.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qoa.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dfz.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mxs.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bqd.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://njx.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://zpl.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ayb.birdmap.top

PHP:  array_reverse($arr);
来源：http://rnl.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wtz.cashguo.top

TS:   [...arr].reverse();
来源：http://pcq.snrcjt.cn

Java: Collections.reverse(list);
来源：http://vnm.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://pwt.yj20258.top

Ruby: arr.reverse
来源：http://npk.zdqjudy.top

C#:   list.Reverse();
来源：http://zys.vqdsnc.cn

[D12] 查找元素下标
来源：http://pio.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://usc.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zyi.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcj.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwr.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cot.tarul.cn

Go:   slices.Index(arr, x)
来源：http://gau.xylfe.cn

Ruby: arr.index(x)
来源：http://jfz.tarul.cn

C#:   list.IndexOf(x);
来源：http://blw.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://etl.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmd.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gnn.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://lef.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://wrv.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kmn.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ifs.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sza.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mqi.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://jhu.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lur.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://neq.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://brn.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://ilb.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eid.aizwys.cn

Go:   // 手写循环
来源：http://iqt.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://dhp.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://oph.cheryme.top

[D15] 去重
来源：http://qji.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mor.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://hmg.hesvh.cn

JS:   [...new Set(arr)]
来源：http://ygd.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://kca.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rua.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://dge.9152youxi.cn

Ruby: arr.uniq
来源：http://kfe.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://xto.nanxinkj.top

[D16] 求和与平均值
来源：http://xsp.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ozn.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qoa.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryi.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ahu.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wfz.hesvh.cn

Go:   // 手写循环累加
来源：http://qzt.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tqu.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://qxh.tian-w.cn

[D17] 最大值与最小值
来源：http://pkq.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://qrl.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://xip.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cin.yvedp.cn

TS:   Math.max(...arr);
来源：http://ugd.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ivj.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://elo.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://afb.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://ijt.cheryme.top

[D18] 扁平化嵌套数组
来源：http://gsw.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yxf.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://wmq.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ged.cqqwz.cn

TS:   nested.flat();
来源：http://dky.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cfo.gogol.net.cn

Go:   // 手写双层循环
来源：http://llc.yvedp.cn

Ruby: nested.flatten
来源：http://kvz.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://vbn.jqgfzy.top

[D19] 按字段分组
来源：http://qwp.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yms.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lnk.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dyo.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nvf.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vak.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://xag.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://inp.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hay.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://bdu.shzxlz.cn

Py:   Counter(arr)
来源：http://zwg.ivvv.top

PHP:  array_count_values($arr);
来源：http://pnm.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qad.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxv.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rcc.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://vda.aibaodan.cn

Ruby: arr.tally
来源：http://tll.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://etn.wangdashe.top

[D21] 判断是否包含某元素
来源：http://vgx.yuanzhike.top

Py:   x in arr
来源：http://dxa.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://wej.c1oappe.top

JS:   arr.includes(x)
来源：http://moi.tian-w.cn

TS:   arr.includes(x)
来源：http://oob.gzhubu.top

Java: list.contains(x)
来源：http://axh.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://ahp.iojbl.cn

Ruby: arr.include?(x)
来源：http://ygy.nanxuanxn.top

C#:   list.Contains(x)
来源：http://zjs.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://btb.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cod.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dlv.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brg.quarkkingdee.top

TS:   [...arr];
来源：http://vzj.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://oka.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://ocj.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://mgq.jqgfzy.top

C#:   new List<int>(list);
来源：http://ldd.cqqwz.cn

[D23] reduce 累积计算
来源：http://yyf.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ics.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqd.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://onv.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://luf.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ypp.tarul.cn

Go:   // 手写循环
来源：http://qqj.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tnq.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ser.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://hda.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ghb.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vqi.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zqi.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bot.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oqo.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldm.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://joo.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pcl.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://rhe.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rqz.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://elx.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wag.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kcg.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nxe.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pny.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tqi.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ium.jinqigufen.top

[D26] 数组转字符串
来源：http://vja.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://yjg.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://ebw.sufxvd.cn

JS:   arr.join(", ")
来源：http://gin.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://zpc.redwolf501.top

Java: String.join(", ", list)
来源：http://qzi.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://apy.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://mdu.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://agh.c1oappe.top

================================================================================
来源：http://mrp.chenjidiqi.icu

E. 字符串处理
来源：http://yrd.hammf.cn

================================================================================
来源：http://btn.jinqigfzy.top

[E01] 拼接字符串
来源：http://yax.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ick.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rjl.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sah.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sry.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jwc.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tpg.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wnb.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://osu.daria6918.cn

[E02] 重复字符串
来源：http://vqu.nwbrower.top

Py:   "ab" * 3
来源：http://qlz.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://fmz.aizwys.cn

JS:   "ab".repeat(3)
来源：http://zgr.hammf.cn

TS:   "ab".repeat(3)
来源：http://jiv.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://ial.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://bzf.316326.xyz

Ruby: "ab" * 3
来源：http://ggj.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dia.gotoacloud.top

[E03] 截取子串
来源：http://ojn.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nzw.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://msu.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tqp.yj20258.top

TS:   s.slice(1, 4)
来源：http://cnt.hysaishi.cn

Java: s.substring(1, 4)
来源：http://gjt.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://was.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://hmw.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://doo.fktsv.cn

[E04] 查找子串位置
来源：http://cwz.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://nin.tian-w.cn

PHP:  strpos($s, "x");
来源：http://ure.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lhm.jianghu66.top

TS:   s.indexOf("x")
来源：http://nns.zhoulong.xyz

Java: s.indexOf("x")
来源：http://cmo.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://fuh.guowangkeji.top

Ruby: s.index("x")
来源：http://ptu.xuanzx.com

C#:   s.IndexOf("x")
来源：http://odx.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tof.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipq.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yis.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfd.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ytv.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aag.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bgk.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lvv.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sph.birdmap.top

[E06] 替换子串
来源：http://bvj.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cit.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://hmt.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysm.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://rfs.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://opl.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xdm.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://udk.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://hcx.hesvh.cn

[E07] 按分隔符拆分
来源：http://nvo.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pgk.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ydp.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vlf.hcnkem.com

TS:   s.split(",")
来源：http://noz.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wep.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qks.yj202588.top

Ruby: s.split(",");  s.split
来源：http://kgl.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ntx.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://dhm.nwbrower.top

Py:   ",".join(items)
来源：http://vym.cdnleiting.top

PHP:  implode(",", $items);
来源：http://ztk.aibaodan.cn

JS:   items.join(",")
来源：http://uqe.jinghuilouyu.cn

TS:   items.join(",")
来源：http://aod.quarkkingdee.top

Java: String.join(",", items)
来源：http://hsd.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://yfj.jqgfzy.top

Ruby: items.join(",")
来源：http://jvs.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://qaq.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://otc.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nsi.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://koq.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://gok.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://kmp.fengsongda.top


<!-- 参考信息 -->