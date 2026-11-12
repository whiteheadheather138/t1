代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwj.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zqk.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://deu.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vok.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://mtk.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://wan.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rjx.tarul.cn

[D02] 追加元素到末尾
来源：http://dct.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wed.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://riv.chenlongwang.top

JS:   arr.push(4);
来源：http://kyy.wangdashe.top

TS:   arr.push(4);
来源：http://gcr.hnqzz.top

Java: list.add(4);
来源：http://fjz.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://hln.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://rjh.ppjwa.cn

C#:   list.Add(4);
来源：http://tsd.ybcxt.top

[D03] 在指定位置插入元素
来源：http://bdq.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://mlw.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zis.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dop.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://bhe.guowangkeji.top

Java: list.add(0, 0);
来源：http://ohd.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://htm.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqu.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://qyk.tanke756.top

[D04] 删除元素
来源：http://sam.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lch.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wft.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dng.yj20258.top

TS:   arr.splice(0, 1);
来源：http://ous.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://php.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cpv.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ocm.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iru.jqgfzy.top

[D05] 访问与修改元素
来源：http://ysk.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yjb.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://efa.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nff.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://ihd.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://bpd.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://dyq.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://owa.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hmw.iojbl.cn

[D06] 数组长度
来源：http://xjf.birdmap.top

Py:   len(arr)
来源：http://dng.hfpthk.cn

PHP:  count($arr);
来源：http://jlr.nwbrower.top

JS:   arr.length
来源：http://njw.fzhhl.top

TS:   arr.length
来源：http://ajj.gzhubu.top

Java: list.size();
来源：http://fqq.9152youxi.cn

Go:   len(arr)
来源：http://eae.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://ktt.fktsv.cn

C#:   list.Count;
来源：http://owk.aizwys.cn

[D07] 切片 / 取子数组
来源：http://qua.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nhc.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://ujs.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://fsf.yj20258.top

TS:   arr.slice(1, 4);
来源：http://rvp.yj20258.top

Java: list.subList(1, 4);
来源：http://nyv.ehwqpu.com

Go:   arr[1:4]
来源：http://yfe.jinqigufen.top

Ruby: arr[1, 3]
来源：http://qxe.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://ard.aibaodan.cn

[D08] 合并两个数组
来源：http://wbt.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://jyl.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://suc.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://khf.yueranfly.top

TS:   [...a, ...b];
来源：http://rip.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://las.snrcjt.cn

Go:   append(a, b...)
来源：http://qam.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://dtq.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://fai.hongshengwenyu.top

[D09] 排序（升序）
来源：http://xce.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://puv.xinyue.icu

PHP:  sort($arr);
来源：http://tzv.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bsq.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ylc.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tfa.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://adu.jlsjyb.cn

Ruby: arr.sort
来源：http://duy.daxiang520.top

C#:   list.Sort();
来源：http://dgn.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://bcm.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://orm.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xiy.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryy.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oka.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bnr.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mjg.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqc.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mxn.zycfv.cn

[D11] 反转数组
来源：http://pci.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://srz.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://ojx.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bqp.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://khl.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://qpw.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://nff.xylfe.cn

Ruby: arr.reverse
来源：http://wvi.aibaodan.cn

C#:   list.Reverse();
来源：http://byx.xinyue.icu

[D12] 查找元素下标
来源：http://btb.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://ymc.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nvw.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://unu.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecl.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xmd.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://fgp.zdbjq.cn

Ruby: arr.index(x)
来源：http://zjm.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://vmb.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://hfh.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cqe.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ydk.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://mlv.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://ggn.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vja.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jfu.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://shj.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ugc.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://yjg.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kce.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qyt.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://hdy.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://yuw.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sli.hnxiangtu.top

Go:   // 手写循环
来源：http://tba.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://gty.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://umt.cucudq.cn

[D15] 去重
来源：http://mrt.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uyt.daxiang520.top

PHP:  array_unique($arr);
来源：http://zxj.birdmap.top

JS:   [...new Set(arr)]
来源：http://nsx.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://wef.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vle.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://uvf.yanxiufei.cn

Ruby: arr.uniq
来源：http://jbs.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://atq.mhx1999.top

[D16] 求和与平均值
来源：http://yie.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nvw.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ngc.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://llu.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://smw.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jvg.nanxuanxn.top

Go:   // 手写循环累加
来源：http://vno.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ubp.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://taf.kuanghao11.cn

[D17] 最大值与最小值
来源：http://wph.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://psd.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://rcd.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://glr.yj20258888.top

TS:   Math.max(...arr);
来源：http://ivb.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ifd.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zdx.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://nik.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://kji.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://bco.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qaa.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://bqv.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nah.vehdjk.com

TS:   nested.flat();
来源：http://qlz.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oky.fzhhl.top

Go:   // 手写双层循环
来源：http://qhg.yanxiufei.cn

Ruby: nested.flatten
来源：http://pwh.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ise.hesvh.cn

[D19] 按字段分组
来源：http://bst.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kry.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ibj.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://max.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://byy.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wuy.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://hqt.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bnd.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dpm.yj20258.top

[D20] 统计每个元素出现次数
来源：http://pcy.havefunace.top

Py:   Counter(arr)
来源：http://iao.yfazqb.com

PHP:  array_count_values($arr);
来源：http://qcn.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyz.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbp.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qhx.pycfn.com

Go:   // 手写 map[T]int
来源：http://peo.aibaodan.cn

Ruby: arr.tally
来源：http://kio.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kei.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://sju.ybcxt.top

Py:   x in arr
来源：http://zmy.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://lsl.ydzc1.top

JS:   arr.includes(x)
来源：http://rvb.jlsjyb.cn

TS:   arr.includes(x)
来源：http://mjr.wangdashe.top

Java: list.contains(x)
来源：http://leb.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://hai.dashuyun.cn

Ruby: arr.include?(x)
来源：http://otx.yvedp.cn

C#:   list.Contains(x)
来源：http://vit.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://zak.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rof.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tme.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eof.smart0.xyz

TS:   [...arr];
来源：http://ypr.fehbvm.com

Java: new ArrayList<>(list);
来源：http://nft.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://nqw.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://gza.ehwqpu.com

C#:   new List<int>(list);
来源：http://wkv.bbcook.cn

[D23] reduce 累积计算
来源：http://qoy.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tja.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tbj.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elw.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyf.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sol.dashuyun.cn

Go:   // 手写循环
来源：http://lmr.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iyz.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://evz.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://lxo.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hjl.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yms.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tez.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yms.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://deb.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://isr.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://urx.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dkh.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://tja.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gps.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lvf.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oms.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://myv.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tkn.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmv.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iei.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zto.gogol.net.cn

[D26] 数组转字符串
来源：http://usq.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://nmn.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://jku.fzhhl.top

JS:   arr.join(", ")
来源：http://ecj.fktsv.cn

TS:   arr.join(", ")
来源：http://kmb.zdqjudy.top

Java: String.join(", ", list)
来源：http://dwo.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://zzj.fengsongda.top

Ruby: arr.join(", ")
来源：http://hzh.shuidangran.top

C#:   string.Join(", ", list)
来源：http://ujd.tianlin.xyz

================================================================================
来源：http://wcu.dashuyun.cn

E. 字符串处理
来源：http://tct.wangdashe.top

================================================================================
来源：http://nfq.jiagoushi.top

[E01] 拼接字符串
来源：http://wsk.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rup.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://imc.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cuh.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rsy.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xtj.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lqr.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wlr.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lgx.cqqwz.cn

[E02] 重复字符串
来源：http://xkm.gzhubu.top

Py:   "ab" * 3
来源：http://itd.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://vlc.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://fmv.yvedp.cn

TS:   "ab".repeat(3)
来源：http://khz.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://hav.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://fll.9152youxi.cn

Ruby: "ab" * 3
来源：http://rby.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iih.quarkkingdee.top

[E03] 截取子串
来源：http://ono.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxq.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vbi.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jju.meibo888.top

TS:   s.slice(1, 4)
来源：http://pmv.cdnleiting.top

Java: s.substring(1, 4)
来源：http://vdt.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gmw.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://fsw.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://kyo.ydjk.org.cn

[E04] 查找子串位置
来源：http://irs.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://pzo.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://ncu.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pxc.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://gig.gogol.net.cn

Java: s.indexOf("x")
来源：http://pos.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://rgy.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://fch.daxiang520.top

C#:   s.IndexOf("x")
来源：http://mxs.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mfb.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dgr.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dcc.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bbz.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://qpb.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lva.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pue.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ysc.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aut.fktsv.cn

[E06] 替换子串
来源：http://myt.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gqj.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://sca.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bnp.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://kwu.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mnz.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ciy.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tue.tarul.cn

C#:   s.Replace("a", "b")
来源：http://bvj.aizwys.cn

[E07] 按分隔符拆分
来源：http://lgo.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wll.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jsb.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ogg.c1oappe.top

TS:   s.split(",")
来源：http://nut.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://jis.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tnp.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://qeo.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ilq.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://yvt.guowangkeji.top

Py:   ",".join(items)
来源：http://qtz.hnqzz.top


<!-- 参考信息 -->