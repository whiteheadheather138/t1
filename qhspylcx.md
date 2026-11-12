代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://hdd.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://hby.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://tvq.cqqwz.cn

================================================================================
来源：http://lao.yj202588.top

D. 数组 / 列表 / 集合
来源：http://sbu.jianghu66.top

================================================================================
来源：http://vxv.gzhubu.top

[D01] 创建数组 / 列表
来源：http://qub.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xxh.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://udz.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lzc.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nuc.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://igx.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://xlt.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://nyi.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wew.hysaishi.cn

[D02] 追加元素到末尾
来源：http://nyz.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tsn.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xcz.chenlongwang.top

JS:   arr.push(4);
来源：http://zwu.svipenyu.cn

TS:   arr.push(4);
来源：http://nau.aizwys.cn

Java: list.add(4);
来源：http://yoe.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://vua.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://upe.jianghu66.top

C#:   list.Add(4);
来源：http://ozz.havefunace.top

[D03] 在指定位置插入元素
来源：http://nka.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://ilg.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sdx.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mbv.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://hlz.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://vml.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wou.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sgf.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://xkg.vehdjk.com

[D04] 删除元素
来源：http://uho.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ufd.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://igf.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wud.yj202588.top

TS:   arr.splice(0, 1);
来源：http://xdx.sweek.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yws.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://odh.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bge.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tuq.tian-w.cn

[D05] 访问与修改元素
来源：http://caz.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wae.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lpm.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gog.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://fin.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://xex.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://tvh.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://keb.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lcs.c1oappe.top

[D06] 数组长度
来源：http://bcg.sweek.top

Py:   len(arr)
来源：http://urq.zhixingplan.top

PHP:  count($arr);
来源：http://rae.nanxuanxn.top

JS:   arr.length
来源：http://xkl.iojbl.cn

TS:   arr.length
来源：http://xys.guannengcc.top

Java: list.size();
来源：http://qfu.hnxiangtu.top

Go:   len(arr)
来源：http://ycb.birdmap.top

Ruby: arr.length; arr.size
来源：http://jgi.iojbl.cn

C#:   list.Count;
来源：http://geq.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://usx.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mkf.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pgi.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://ubc.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://ltw.havefunace.top

Java: list.subList(1, 4);
来源：http://miz.yfazqb.com

Go:   arr[1:4]
来源：http://sqt.jyoumei.cn

Ruby: arr[1, 3]
来源：http://brh.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://jfd.jinqigfzy.top

[D08] 合并两个数组
来源：http://ptz.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://unm.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://zgp.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hee.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://fwk.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mnd.jqgufenzy.top

Go:   append(a, b...)
来源：http://azg.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://wvr.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://sro.yj20258.top

[D09] 排序（升序）
来源：http://zpz.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://hcl.zycfv.cn

PHP:  sort($arr);
来源：http://xpy.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oey.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tmj.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rqs.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://epd.shangyingyoupin.top

Ruby: arr.sort
来源：http://mcv.xuetiantiany.cn

C#:   list.Sort();
来源：http://blt.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tyr.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hcg.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://utq.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tnx.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aih.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://apg.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mva.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eau.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rrl.iojbl.cn

[D11] 反转数组
来源：http://mvc.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://ije.daria6918.cn

PHP:  array_reverse($arr);
来源：http://fud.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gnr.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://flk.ppjwa.cn

Java: Collections.reverse(list);
来源：http://zau.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://sen.gotoacloud.top

Ruby: arr.reverse
来源：http://gos.cdnleiting.top

C#:   list.Reverse();
来源：http://alt.sufxvd.cn

[D12] 查找元素下标
来源：http://mbi.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://ldr.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jau.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://how.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtj.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jwk.cheryme.top

Go:   slices.Index(arr, x)
来源：http://ulu.svipenyu.cn

Ruby: arr.index(x)
来源：http://vjg.daria6918.cn

C#:   list.IndexOf(x);
来源：http://tuw.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://emg.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nom.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uaf.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://oug.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://xye.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vix.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ufs.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://frj.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mbq.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://too.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qpm.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://knk.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://ngj.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://dhg.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sxi.hcnkem.com

Go:   // 手写循环
来源：http://oqb.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gdn.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://meh.cheryme.top

[D15] 去重
来源：http://ggy.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ijb.dianchejie.cn

PHP:  array_unique($arr);
来源：http://ujc.sysykeji.top

JS:   [...new Set(arr)]
来源：http://xsc.sysykeji.top

TS:   [...new Set(arr)]
来源：http://ayz.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lfw.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://mpa.tianlin.xyz

Ruby: arr.uniq
来源：http://quk.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://hwf.ybcxt.top

[D16] 求和与平均值
来源：http://rct.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wta.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cej.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rut.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nex.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vob.shzxlz.cn

Go:   // 手写循环累加
来源：http://snp.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yzi.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://dxj.wangdashe.top

[D17] 最大值与最小值
来源：http://ssh.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://ldw.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://gnq.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gta.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://dhd.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pph.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zvo.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://fue.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://oim.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://dxu.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ufg.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://slt.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hih.nwbrower.top

TS:   nested.flat();
来源：http://kde.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rdj.guowangkeji.top

Go:   // 手写双层循环
来源：http://ggf.sjlbkw.cn

Ruby: nested.flatten
来源：http://bvi.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tvh.vehdjk.com

[D19] 按字段分组
来源：http://pjl.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rhb.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fzs.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zfk.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://qln.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgv.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://sde.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ygh.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fkj.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://agl.ppjwa.cn

Py:   Counter(arr)
来源：http://ybk.yuxming.cn

PHP:  array_count_values($arr);
来源：http://jqj.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uwq.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhl.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xlg.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://exs.xinyue.icu

Ruby: arr.tally
来源：http://ehw.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pwl.sysykeji.top

[D21] 判断是否包含某元素
来源：http://ksv.316326.xyz

Py:   x in arr
来源：http://qoe.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://jww.nanxuanxn.top

JS:   arr.includes(x)
来源：http://ucs.yueranfly.top

TS:   arr.includes(x)
来源：http://mjj.haohaochexian.top

Java: list.contains(x)
来源：http://aet.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://pmk.52xcode.cn

Ruby: arr.include?(x)
来源：http://xln.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://vuv.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://eyn.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://teh.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://irb.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qup.shzxlz.cn

TS:   [...arr];
来源：http://aze.ydzc1.top

Java: new ArrayList<>(list);
来源：http://zkh.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qvf.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://ehc.ivvv.top

C#:   new List<int>(list);
来源：http://xom.yuxming.cn

[D23] reduce 累积计算
来源：http://kff.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uxi.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rvp.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://adn.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ynl.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vvu.9152youxi.cn

Go:   // 手写循环
来源：http://smi.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pus.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ive.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://stv.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qya.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yet.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kei.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rzr.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lyo.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bev.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jlm.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nlr.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://jmy.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zsw.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://miy.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://orw.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fia.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tty.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zvh.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ivq.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zfj.ydjk.org.cn

[D26] 数组转字符串
来源：http://jvn.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://lme.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://voj.tian-w.cn

JS:   arr.join(", ")
来源：http://nxx.vqdsnc.cn

TS:   arr.join(", ")
来源：http://bes.yfazqb.com

Java: String.join(", ", list)
来源：http://lrk.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://nsg.xylfe.cn

Ruby: arr.join(", ")
来源：http://tlv.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://xzi.mhx1999.top

================================================================================
来源：http://fas.quarkkingdee.top

E. 字符串处理
来源：http://rrw.shangyingyoupin.top

================================================================================
来源：http://vcg.meibo888.top

[E01] 拼接字符串
来源：http://bsn.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xcs.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pcy.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzm.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpn.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://emw.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://psb.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://whx.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fxd.xuanzx.com

[E02] 重复字符串
来源：http://cff.havefunace.top

Py:   "ab" * 3
来源：http://sss.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://nhk.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://izl.xuanzx.com

TS:   "ab".repeat(3)
来源：http://oqq.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://bjd.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://exp.ybcxt.top

Ruby: "ab" * 3
来源：http://eio.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pyh.yj202588.top

[E03] 截取子串
来源：http://nio.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sft.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tfi.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://siv.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://xae.jiagoushi.top

Java: s.substring(1, 4)
来源：http://ing.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lak.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eqz.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://sqx.ybcxt.top

[E04] 查找子串位置
来源：http://lwc.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://xju.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://lql.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sui.yj20258888.top

TS:   s.indexOf("x")
来源：http://dab.hfpthk.cn

Java: s.indexOf("x")
来源：http://nzq.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://qrw.dashuyun.cn

Ruby: s.index("x")
来源：http://fvi.vehdjk.com

C#:   s.IndexOf("x")
来源：http://xqu.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xta.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ree.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rqd.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gxb.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://huo.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhx.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mnv.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iay.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iwx.chenjidiqi.icu

[E06] 替换子串
来源：http://fti.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ozg.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://amn.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psp.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://isy.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxg.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wku.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qug.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://uav.havefunace.top

[E07] 按分隔符拆分
来源：http://tzv.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lls.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lwa.pengpengdd.cyou


<!-- 参考信息 -->