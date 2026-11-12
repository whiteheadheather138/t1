代发 wailian999

C#:   list.Insert(0, 0);
来源：http://jfv.cashguo.top

[D04] 删除元素
来源：http://dot.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pdg.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oet.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://faz.yj20258.top

TS:   arr.splice(0, 1);
来源：http://vgw.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uep.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ldn.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pov.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oav.chenlongwang.top

[D05] 访问与修改元素
来源：http://cwh.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lyr.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://egb.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wqb.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://yta.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://bfb.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://hdb.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jey.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vvx.yonumen.top

[D06] 数组长度
来源：http://ane.jlsjyb.cn

Py:   len(arr)
来源：http://lqq.mhx1999.top

PHP:  count($arr);
来源：http://dfb.sweek.top

JS:   arr.length
来源：http://igo.yvedp.cn

TS:   arr.length
来源：http://xab.zhongyouzk.top

Java: list.size();
来源：http://zip.yvedp.cn

Go:   len(arr)
来源：http://die.fzhhl.top

Ruby: arr.length; arr.size
来源：http://guz.hfpthk.cn

C#:   list.Count;
来源：http://vrz.hcnkem.com

[D07] 切片 / 取子数组
来源：http://vtz.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jew.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://vcn.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://vde.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://irs.hesvh.cn

Java: list.subList(1, 4);
来源：http://kqw.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://inl.cashguo.top

Ruby: arr[1, 3]
来源：http://yof.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://rgh.cheryme.top

[D08] 合并两个数组
来源：http://cij.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://rnk.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://lla.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hnh.ivvv.top

TS:   [...a, ...b];
来源：http://vcj.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kvc.hywenlv.cn

Go:   append(a, b...)
来源：http://fll.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://jtz.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://pql.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://wla.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://kyo.ctjpmb.com

PHP:  sort($arr);
来源：http://qnw.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ilk.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://faj.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mms.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ehf.jlsjyb.cn

Ruby: arr.sort
来源：http://vfa.jinqigfzy.top

C#:   list.Sort();
来源：http://ead.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ljb.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://joa.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://szl.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfp.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ykm.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qmh.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sks.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ash.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ybw.zhengqikj.top

[D11] 反转数组
来源：http://ude.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lpf.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://qsu.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ugh.wangdashe.top

TS:   [...arr].reverse();
来源：http://bqa.wangdashe.top

Java: Collections.reverse(list);
来源：http://cjv.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://yse.jqgfzy.top

Ruby: arr.reverse
来源：http://upw.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://zap.sjlbkw.cn

[D12] 查找元素下标
来源：http://cvu.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://uxs.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bpw.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcv.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ath.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rsj.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://jtz.yanxiufei.cn

Ruby: arr.index(x)
来源：http://unk.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://xox.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://bjd.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yik.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hjo.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://glb.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://rvi.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ued.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lgw.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://czz.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dwq.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://ykf.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ukn.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://llb.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://iju.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://dqd.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://flw.mhx1999.top

Go:   // 手写循环
来源：http://fiu.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://qfa.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yny.ywan-chungtsiang.top

[D15] 去重
来源：http://hvm.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zjq.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://nuv.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://fjd.tian-w.cn

TS:   [...new Set(arr)]
来源：http://kgi.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hhr.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lwh.tian-w.cn

Ruby: arr.uniq
来源：http://yjo.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://zml.mhx1999.top

[D16] 求和与平均值
来源：http://iyp.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jub.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kbb.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyw.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ljb.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ivm.fzhhl.top

Go:   // 手写循环累加
来源：http://tvm.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mim.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://pkc.aibaodan.cn

[D17] 最大值与最小值
来源：http://vyf.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://ymr.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://uwu.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://auv.guannengcc.top

TS:   Math.max(...arr);
来源：http://obc.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wgq.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exc.birdmap.top

Ruby: arr.max;  arr.min
来源：http://nwx.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://aas.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://ajr.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wgj.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://vun.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lwu.gzhubu.top

TS:   nested.flat();
来源：http://egc.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jng.nwbrower.top

Go:   // 手写双层循环
来源：http://pys.hnqzz.top

Ruby: nested.flatten
来源：http://lsg.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uot.havefunace.top

[D19] 按字段分组
来源：http://jty.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tom.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eui.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qhk.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://olc.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nit.yj202588.top

Go:   // 手写 map[string][]T
来源：http://lau.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://awv.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxl.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://gsv.aizwys.cn

Py:   Counter(arr)
来源：http://djy.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://hht.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aod.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pgi.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mcl.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://gwx.chenzaomai.com

Ruby: arr.tally
来源：http://qso.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hdg.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://peh.havefunace.top

Py:   x in arr
来源：http://znu.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://clx.ctjpmb.com

JS:   arr.includes(x)
来源：http://iab.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://aym.cucudq.cn

Java: list.contains(x)
来源：http://sss.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://rjg.havefunace.top

Ruby: arr.include?(x)
来源：http://oia.ivvv.top

C#:   list.Contains(x)
来源：http://nzl.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://tik.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://opb.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://snw.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gac.fehbvm.com

TS:   [...arr];
来源：http://nkg.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://zes.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ttg.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://ovo.cucudq.cn

C#:   new List<int>(list);
来源：http://vpr.hesvh.cn

[D23] reduce 累积计算
来源：http://ecx.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jrs.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ukl.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eij.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqw.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xug.0kj1m.cn

Go:   // 手写循环
来源：http://njp.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wbw.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kmx.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://rlc.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://drf.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pep.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://szr.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jnw.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hrf.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://flf.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsd.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jxq.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://qxl.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://atx.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zcw.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mzr.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hpm.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rbo.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mof.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bsv.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ijz.zhoulong.xyz

[D26] 数组转字符串
来源：http://zfl.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://dwh.yonumen.top

PHP:  implode(", ", $arr);
来源：http://utc.fzhhl.top

JS:   arr.join(", ")
来源：http://ula.gogol.net.cn

TS:   arr.join(", ")
来源：http://xan.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://rzz.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://fzh.chenzaomai.com

Ruby: arr.join(", ")
来源：http://lud.52xcode.cn

C#:   string.Join(", ", list)
来源：http://lag.feifeiyinyue.top

================================================================================
来源：http://bza.ywan-chungtsiang.top

E. 字符串处理
来源：http://ooh.hesvh.cn

================================================================================
来源：http://qre.havefunace.top

[E01] 拼接字符串
来源：http://vpp.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jvl.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tvy.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zad.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zan.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fnu.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xmv.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vfx.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kln.xylfe.cn

[E02] 重复字符串
来源：http://luh.mhx1999.top

Py:   "ab" * 3
来源：http://efg.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://qgs.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://pku.hammf.cn

TS:   "ab".repeat(3)
来源：http://acm.jyoumei.cn

Java: "ab".repeat(3)
来源：http://xst.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://snn.yj20258888.top

Ruby: "ab" * 3
来源：http://wrv.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://brw.jinghuilouyu.cn

[E03] 截取子串
来源：http://oyn.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rsb.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mbs.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jcl.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://ghd.xinyue.icu

Java: s.substring(1, 4)
来源：http://tiy.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oef.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://gly.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://dcc.gaohongyu789.top

[E04] 查找子串位置
来源：http://umd.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://kmo.xylfe.cn

PHP:  strpos($s, "x");
来源：http://bbb.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ewa.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://edj.hnxiangtu.top

Java: s.indexOf("x")
来源：http://ceq.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://rqm.52xcode.cn

Ruby: s.index("x")
来源：http://lda.sysykeji.top

C#:   s.IndexOf("x")
来源：http://wez.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ovj.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oxe.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yvw.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://crp.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vga.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pkc.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://btz.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://htp.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lcv.ivvv.top

[E06] 替换子串
来源：http://gju.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ipr.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://lwk.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwb.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://ixh.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwk.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ocp.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://stk.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://tzm.pycfn.com

[E07] 按分隔符拆分
来源：http://ksb.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zmj.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rvn.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://psd.nwbrower.top

TS:   s.split(",")
来源：http://qsb.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://mjf.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lam.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://kvz.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vwq.tanke756.top

[E08] 数组按分隔符合并
来源：http://mku.yangfankeji.com

Py:   ",".join(items)
来源：http://dcx.hywenlv.cn

PHP:  implode(",", $items);
来源：http://pjm.yangfankeji.com

JS:   items.join(",")
来源：http://bok.zycfv.cn

TS:   items.join(",")
来源：http://esi.xziqi.cn

Java: String.join(",", items)
来源：http://xho.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://xdz.hysaishi.cn

Ruby: items.join(",")
来源：http://lzm.ydzc1.top

C#:   string.Join(",", items)
来源：http://hhl.cqqwz.cn

[E09] 去除所有空白字符
来源：http://mfk.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://msx.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dec.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://wsl.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://chd.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://fgo.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tkb.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://dlw.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yqo.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://sjv.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://adn.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rdd.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://wcb.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://ysm.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://svj.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fhd.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ucf.fanxiaobao.xyz


<!-- 参考信息 -->