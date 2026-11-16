代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://vpt.zhoulong.xyz

Java: list.add(0, 0);
来源：http://zvj.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ukk.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ynk.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://nbk.jinghuilouyu.cn

[D04] 删除元素
来源：http://moa.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oqi.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ufm.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wlk.hammf.cn

TS:   arr.splice(0, 1);
来源：http://ctl.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ztv.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shg.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jmx.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ofz.jlsjyb.cn

[D05] 访问与修改元素
来源：http://miz.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cah.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rsz.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://upu.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://rru.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://evs.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://qzj.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://boy.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gre.yj20258.top

[D06] 数组长度
来源：http://mwk.feifeiyinyue.top

Py:   len(arr)
来源：http://dzy.andypj.xyz

PHP:  count($arr);
来源：http://ndf.vehdjk.com

JS:   arr.length
来源：http://tke.9152youxi.cn

TS:   arr.length
来源：http://des.0kj1m.cn

Java: list.size();
来源：http://jxq.cashguo.top

Go:   len(arr)
来源：http://fvu.hammf.cn

Ruby: arr.length; arr.size
来源：http://gqz.wangdashe.top

C#:   list.Count;
来源：http://hfe.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://iug.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nmf.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://vqg.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://gze.pycfn.com

TS:   arr.slice(1, 4);
来源：http://wpd.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://yhm.daxiang520.top

Go:   arr[1:4]
来源：http://arq.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://boq.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://bca.gzhubu.top

[D08] 合并两个数组
来源：http://drq.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://isk.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://ibw.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vll.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://kdr.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oqv.feifeiyinyue.top

Go:   append(a, b...)
来源：http://ves.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://byr.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://ptb.quarkkingdee.top

[D09] 排序（升序）
来源：http://tyj.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://ipn.xinyue.icu

PHP:  sort($arr);
来源：http://ibr.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://skc.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ujr.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qju.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wnz.xziqi.cn

Ruby: arr.sort
来源：http://mgd.cdnleiting.top

C#:   list.Sort();
来源：http://aux.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jiz.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ynf.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ycz.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpl.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jnm.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tej.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rai.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ngx.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ksv.0kj1m.cn

[D11] 反转数组
来源：http://pyw.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://ffu.birdmap.top

PHP:  array_reverse($arr);
来源：http://waj.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kwz.fktsv.cn

TS:   [...arr].reverse();
来源：http://qdl.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://mdq.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://vcx.tarul.cn

Ruby: arr.reverse
来源：http://vvt.gotoacloud.top

C#:   list.Reverse();
来源：http://aec.zdbjq.cn

[D12] 查找元素下标
来源：http://xzg.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://eye.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xwy.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cuu.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://odl.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kee.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://yve.xinyue.icu

Ruby: arr.index(x)
来源：http://rnv.shuidangran.top

C#:   list.IndexOf(x);
来源：http://iks.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://zjj.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://apg.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zwx.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://tqf.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://ude.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bqf.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hnn.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://sxw.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ura.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://ysy.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qgn.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oxh.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://ofn.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://lpy.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzh.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://xcp.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://vle.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sid.sjlbkw.cn

[D15] 去重
来源：http://kyd.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jmp.yj202588.top

PHP:  array_unique($arr);
来源：http://hts.xylfe.cn

JS:   [...new Set(arr)]
来源：http://zkk.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://knb.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zin.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://usl.ydjk.org.cn

Ruby: arr.uniq
来源：http://tvx.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://umk.smart0.xyz

[D16] 求和与平均值
来源：http://tup.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ass.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aoa.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddy.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yuj.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nvd.cdnleiting.top

Go:   // 手写循环累加
来源：http://whd.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jcy.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://mjn.nwbrower.top

[D17] 最大值与最小值
来源：http://gcf.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://ewk.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://wqj.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sji.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://fns.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://byp.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://skh.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://knb.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://vgt.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://nas.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://icx.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://ccu.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lqt.52xcode.cn

TS:   nested.flat();
来源：http://xsa.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lxd.guannengcc.top

Go:   // 手写双层循环
来源：http://kib.jianghu66.top

Ruby: nested.flatten
来源：http://kyf.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fxh.redwolf501.top

[D19] 按字段分组
来源：http://kaz.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bxk.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://brl.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ort.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vzc.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ata.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://tlm.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpf.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hql.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://eyz.zhoulong.xyz

Py:   Counter(arr)
来源：http://hyu.uphjek.com

PHP:  array_count_values($arr);
来源：http://rwi.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esu.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://puo.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gmr.hesvh.cn

Go:   // 手写 map[T]int
来源：http://dvw.xinyue.icu

Ruby: arr.tally
来源：http://dnd.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jcp.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://dzc.fengsongda.top

Py:   x in arr
来源：http://qur.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://ita.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://pto.hnxiangtu.top

TS:   arr.includes(x)
来源：http://iqp.yangfankeji.com

Java: list.contains(x)
来源：http://kjh.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://xke.pycfn.com

Ruby: arr.include?(x)
来源：http://tgk.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://jgt.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://vpo.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vku.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cbm.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gpv.jianghu66.top

TS:   [...arr];
来源：http://who.316326.xyz

Java: new ArrayList<>(list);
来源：http://agy.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yrk.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://waf.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://orl.wangdashe.top

[D23] reduce 累积计算
来源：http://xyv.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://khk.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ljg.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfu.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njr.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ash.yuxming.cn

Go:   // 手写循环
来源：http://tve.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://irj.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ceb.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://uib.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://syz.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdq.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tvi.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://coh.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dnv.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewe.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dve.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dqj.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://qwa.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tmd.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ccs.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aal.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ngr.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fwg.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ewt.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nhe.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwo.xuanzx.com

[D26] 数组转字符串
来源：http://cyg.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://zyo.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://vbk.yuxming.cn

JS:   arr.join(", ")
来源：http://zkm.yanxiufei.cn

TS:   arr.join(", ")
来源：http://ccn.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://zbr.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://tio.gogol.net.cn

Ruby: arr.join(", ")
来源：http://tto.tarul.cn

C#:   string.Join(", ", list)
来源：http://dup.shanyushiyangtech.top

================================================================================
来源：http://phe.iojbl.cn

E. 字符串处理
来源：http://idr.zhongyouzk.top

================================================================================
来源：http://ilf.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://hzx.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jgq.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jag.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qdx.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://puw.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kpv.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iix.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pgg.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ccp.zhiwuduotai.top

[E02] 重复字符串
来源：http://czx.birdmap.top

Py:   "ab" * 3
来源：http://mmj.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://adr.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://jww.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://kkk.dianchejie.cn

Java: "ab".repeat(3)
来源：http://lyc.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://zzf.quarkkingdee.top

Ruby: "ab" * 3
来源：http://vgw.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tbv.ppjwa.cn

[E03] 截取子串
来源：http://cvv.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tdj.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kux.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://npu.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://obo.jiagoushi.top

Java: s.substring(1, 4)
来源：http://rml.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://put.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://kzj.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://dnt.jyoumei.cn

[E04] 查找子串位置
来源：http://pxi.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://vfx.fengsongda.top

PHP:  strpos($s, "x");
来源：http://gpd.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://equ.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://cjk.zdqjudy.top

Java: s.indexOf("x")
来源：http://tvq.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://wyy.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://slk.yj202588.top

C#:   s.IndexOf("x")
来源：http://bef.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wal.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jfj.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjn.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtu.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yoj.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efl.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tjf.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kaa.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ncu.cheryme.top

[E06] 替换子串
来源：http://faz.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eqm.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://ije.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrw.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://cqz.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhj.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qcb.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhy.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://vkl.daxiang520.top

[E07] 按分隔符拆分
来源：http://haf.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gke.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ekr.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wbo.ybcxt.top

TS:   s.split(",")
来源：http://mao.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://bzx.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tqo.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://tat.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyl.yueranfly.top

[E08] 数组按分隔符合并
来源：http://ycr.cqqwz.cn

Py:   ",".join(items)
来源：http://yhv.jyoumei.cn

PHP:  implode(",", $items);
来源：http://chx.shuidangran.top

JS:   items.join(",")
来源：http://fcs.guannengcc.top

TS:   items.join(",")
来源：http://omp.gogol.net.cn

Java: String.join(",", items)
来源：http://jyr.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://xwb.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://ldn.hywenlv.cn

C#:   string.Join(",", items)
来源：http://qkd.iojbl.cn

[E09] 去除所有空白字符
来源：http://dfp.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://epl.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ryy.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://nbd.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://enr.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://ohh.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cgi.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jno.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://upf.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://vld.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mjz.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oze.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://elv.xuanzx.com


<!-- 参考信息 -->