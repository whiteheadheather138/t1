代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ixv.yj202588.top

Java: list.add(0, 0);
来源：http://hev.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kly.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://guz.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://odb.epnwcf.com

[D04] 删除元素
来源：http://xfe.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dzw.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eaw.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sgp.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://ewz.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gje.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bub.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dxv.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vdy.ydjk.org.cn

[D05] 访问与修改元素
来源：http://rta.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pqj.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tzg.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovh.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://xaz.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://yvm.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://cuf.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ucp.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwr.yj20258.top

[D06] 数组长度
来源：http://wuc.tian-w.cn

Py:   len(arr)
来源：http://lct.zhoulong.xyz

PHP:  count($arr);
来源：http://zen.yj202588.top

JS:   arr.length
来源：http://igt.yuxming.cn

TS:   arr.length
来源：http://bck.shangyingyoupin.top

Java: list.size();
来源：http://zqf.hywenlv.cn

Go:   len(arr)
来源：http://wmv.cashguo.top

Ruby: arr.length; arr.size
来源：http://rid.ehwqpu.com

C#:   list.Count;
来源：http://oig.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://kvj.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nfq.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://yug.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://tld.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://lfn.haohaochexian.top

Java: list.subList(1, 4);
来源：http://cev.xuanzx.com

Go:   arr[1:4]
来源：http://cwv.guowangkeji.top

Ruby: arr[1, 3]
来源：http://lpu.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://wii.hnxiangtu.top

[D08] 合并两个数组
来源：http://ayw.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://dga.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://byd.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rto.ydzc1.top

TS:   [...a, ...b];
来源：http://rif.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dqz.aibaodan.cn

Go:   append(a, b...)
来源：http://aoc.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://nqi.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://bqf.pengpengdd.cyou

[D09] 排序（升序）
来源：http://xzk.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lsb.bbcook.cn

PHP:  sort($arr);
来源：http://sup.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xmj.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mho.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wyj.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://swi.hnxiangtu.top

Ruby: arr.sort
来源：http://tij.jqgfzy.top

C#:   list.Sort();
来源：http://cxx.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ivi.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lkx.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfu.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://umd.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lax.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ibs.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eyu.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://csf.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dgu.sjlbkw.cn

[D11] 反转数组
来源：http://cfj.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://eib.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://ell.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://osc.hcnkem.com

TS:   [...arr].reverse();
来源：http://pgb.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://qzr.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://mjg.ydzc1.top

Ruby: arr.reverse
来源：http://okb.tanke756.top

C#:   list.Reverse();
来源：http://ukz.nanxuanxn.top

[D12] 查找元素下标
来源：http://yks.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://nrw.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cdt.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iax.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vht.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uqq.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://mom.yuanzhike.top

Ruby: arr.index(x)
来源：http://lkg.epnwcf.com

C#:   list.IndexOf(x);
来源：http://lhj.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://sfn.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xfc.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pee.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://rcv.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://its.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://civ.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lgx.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://yhm.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ltg.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://fic.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zfx.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tho.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://sas.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://ukj.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lza.aibaodan.cn

Go:   // 手写循环
来源：http://yle.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://wjn.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://scs.bbcook.cn

[D15] 去重
来源：http://nco.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lvy.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://oht.aizwys.cn

JS:   [...new Set(arr)]
来源：http://rhx.nwbrower.top

TS:   [...new Set(arr)]
来源：http://ljl.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://est.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fom.zhoulong.xyz

Ruby: arr.uniq
来源：http://oxe.tarul.cn

C#:   list.Distinct().ToList()
来源：http://xjx.jlsjyb.cn

[D16] 求和与平均值
来源：http://rkk.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jws.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sms.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbz.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ter.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qzu.tianlin.xyz

Go:   // 手写循环累加
来源：http://pzo.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lxz.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://qlp.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://ztb.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://lgn.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://fzc.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tpo.xuanzx.com

TS:   Math.max(...arr);
来源：http://qtv.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ixk.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://clu.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://wst.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://tft.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://jiu.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aod.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://lcz.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sry.chenzaomai.com

TS:   nested.flat();
来源：http://drt.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ogb.xuanzx.com

Go:   // 手写双层循环
来源：http://adi.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://eal.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ydv.hywenlv.cn

[D19] 按字段分组
来源：http://kco.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rsk.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ebe.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rpl.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fuw.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bgf.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://tub.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ggk.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryl.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://gqp.jqgfzy.top

Py:   Counter(arr)
来源：http://jpk.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://cnq.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://seo.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hxj.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fpf.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://qug.yfazqb.com

Ruby: arr.tally
来源：http://toa.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://goy.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://xoe.zdbjq.cn

Py:   x in arr
来源：http://wvb.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://bmw.zhongyouzk.top

JS:   arr.includes(x)
来源：http://zhn.hnxiangtu.top

TS:   arr.includes(x)
来源：http://anx.yangfankeji.com

Java: list.contains(x)
来源：http://ely.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://jtj.tarul.cn

Ruby: arr.include?(x)
来源：http://ilz.yuanzhike.top

C#:   list.Contains(x)
来源：http://uao.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://scg.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://agi.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wfy.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zhx.bbcook.cn

TS:   [...arr];
来源：http://kua.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://ehb.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://fbl.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://csh.zhongyouzk.top

C#:   new List<int>(list);
来源：http://ksm.yfazqb.com

[D23] reduce 累积计算
来源：http://rhj.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://myz.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ray.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxh.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igd.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://agx.cheryme.top

Go:   // 手写循环
来源：http://dai.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://apu.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tpf.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://oeb.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfg.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://omv.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ycs.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://opv.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zkq.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tge.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cec.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qzn.birdmap.top

[D25] Set 集合去重与交并差
来源：http://rvl.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xij.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gsb.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fxm.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jox.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jwx.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jyz.sweek.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://llh.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jbr.tianlin.xyz

[D26] 数组转字符串
来源：http://pyb.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://tgq.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://wkv.zdbjq.cn

JS:   arr.join(", ")
来源：http://ymp.c1oappe.top

TS:   arr.join(", ")
来源：http://ovi.aizwys.cn

Java: String.join(", ", list)
来源：http://oyj.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://plu.pycfn.com

Ruby: arr.join(", ")
来源：http://had.ydzc1.top

C#:   string.Join(", ", list)
来源：http://slt.jinghuilouyu.cn

================================================================================
来源：http://tsb.feifeiyinyue.top

E. 字符串处理
来源：http://hwe.cucudq.cn

================================================================================
来源：http://bpn.bbcook.cn

[E01] 拼接字符串
来源：http://pmi.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kcy.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xpp.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rog.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gvf.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://owf.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ezw.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cfy.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xye.yongpay.top

[E02] 重复字符串
来源：http://naz.zdqjudy.top

Py:   "ab" * 3
来源：http://rpn.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://ggl.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://ohd.aizwys.cn

TS:   "ab".repeat(3)
来源：http://zym.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://uke.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://wrc.yvedp.cn

Ruby: "ab" * 3
来源：http://ggj.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dqw.smart0.xyz

[E03] 截取子串
来源：http://vhk.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sxa.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dxv.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgy.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://izz.shzxlz.cn

Java: s.substring(1, 4)
来源：http://yhj.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uan.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jvd.yongpay.top

C#:   s.Substring(1, 3)
来源：http://epz.9152youxi.cn

[E04] 查找子串位置
来源：http://any.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://jdv.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://nvk.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://geb.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://fxz.jianghu66.top

Java: s.indexOf("x")
来源：http://npp.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://lrd.jinqigfzy.top

Ruby: s.index("x")
来源：http://pwq.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://sbj.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oev.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cdy.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uur.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rvk.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vrr.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kbh.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://odw.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ucb.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mno.chenjidiqi.icu

[E06] 替换子串
来源：http://ije.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dti.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://ulq.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdn.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://xnr.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cql.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ybd.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tei.birdmap.top

C#:   s.Replace("a", "b")
来源：http://fdu.chenzaomai.com

[E07] 按分隔符拆分
来源：http://hai.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mfw.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uuu.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tzr.quarkkingdee.top

TS:   s.split(",")
来源：http://hzg.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jsu.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hwj.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://uvq.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kte.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://noe.dashuyun.cn

Py:   ",".join(items)
来源：http://bkd.ydzc1.top

PHP:  implode(",", $items);
来源：http://cap.sjlbkw.cn

JS:   items.join(",")
来源：http://dbw.cashguo.top

TS:   items.join(",")
来源：http://yjm.birdmap.top

Java: String.join(",", items)
来源：http://foc.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://lvk.vehdjk.com

Ruby: items.join(",")
来源：http://ejw.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://hmu.jyoumei.cn

[E09] 去除所有空白字符
来源：http://mve.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://brl.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zty.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://ocg.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://nse.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://aqy.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://plk.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://lgb.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ehf.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://pwx.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://krg.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zth.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://xor.havefunace.top


<!-- 参考信息 -->