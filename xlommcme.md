代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://thz.vehdjk.com

Java: list.add(0, 0);
来源：http://uje.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://pbp.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hsk.yonumen.top

C#:   list.Insert(0, 0);
来源：http://ilj.yuxming.cn

[D04] 删除元素
来源：http://sgw.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wcy.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oum.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://psm.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://ovt.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kzb.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yve.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bhx.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uyg.9152youxi.cn

[D05] 访问与修改元素
来源：http://wuh.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xqs.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bnr.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qlj.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://geb.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://xll.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://hpo.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://skk.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wox.vqdsnc.cn

[D06] 数组长度
来源：http://fhm.ywan-chungtsiang.top

Py:   len(arr)
来源：http://rme.zhixingplan.top

PHP:  count($arr);
来源：http://mgn.yonumen.top

JS:   arr.length
来源：http://vcd.xingfuxueyuan.xyz

TS:   arr.length
来源：http://sbz.nwbrower.top

Java: list.size();
来源：http://tbx.tanke756.top

Go:   len(arr)
来源：http://cac.fengsongda.top

Ruby: arr.length; arr.size
来源：http://cex.hesvh.cn

C#:   list.Count;
来源：http://auy.yongpay.top

[D07] 切片 / 取子数组
来源：http://inx.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nbh.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://eie.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://klg.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://lrn.guannengcc.top

Java: list.subList(1, 4);
来源：http://wve.shuidangran.top

Go:   arr[1:4]
来源：http://yvg.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://juz.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://cvf.pycfn.com

[D08] 合并两个数组
来源：http://dss.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://zuw.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://pjk.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pnb.vehdjk.com

TS:   [...a, ...b];
来源：http://dkr.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hdq.jlsjyb.cn

Go:   append(a, b...)
来源：http://gdk.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://iaa.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://ckt.xinyue.icu

[D09] 排序（升序）
来源：http://dxk.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://upv.chenlongwang.top

PHP:  sort($arr);
来源：http://lji.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kkv.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pnk.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://knj.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgb.pengpengdd.cyou

Ruby: arr.sort
来源：http://gpz.yj202588.top

C#:   list.Sort();
来源：http://own.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rla.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mjo.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cyh.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbv.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zjg.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://viv.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bip.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://emw.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ibf.chenzaomai.com

[D11] 反转数组
来源：http://uig.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://vxb.bjfxy.top

PHP:  array_reverse($arr);
来源：http://zdt.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bmy.yuanzhike.top

TS:   [...arr].reverse();
来源：http://ycb.yvedp.cn

Java: Collections.reverse(list);
来源：http://caz.havefunace.top

Go:   slices.Reverse(arr)
来源：http://eib.9152youxi.cn

Ruby: arr.reverse
来源：http://dxf.hysaishi.cn

C#:   list.Reverse();
来源：http://tkx.52xcode.cn

[D12] 查找元素下标
来源：http://zov.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://loj.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zpl.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pat.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pos.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhg.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://zjp.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://vcy.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://osg.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://xgo.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jqf.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mtr.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://ztf.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://zoc.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrs.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oec.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://upv.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vfu.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://hfh.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dns.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mzz.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://jae.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://otn.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dth.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://skt.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xnh.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fez.dianchejie.cn

[D15] 去重
来源：http://tuy.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oly.shzxlz.cn

PHP:  array_unique($arr);
来源：http://cqo.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://jyw.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://ttp.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://igp.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://hvq.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://xud.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://grd.vehdjk.com

[D16] 求和与平均值
来源：http://yyi.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://egc.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jlc.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zkz.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yvl.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xyb.wangdashe.top

Go:   // 手写循环累加
来源：http://vxi.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qpn.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://hzk.pycfn.com

[D17] 最大值与最小值
来源：http://gyj.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://zhr.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://ovv.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwk.zhengqikj.top

TS:   Math.max(...arr);
来源：http://hqq.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lxb.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cry.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://mag.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://spi.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://frz.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://paz.hammf.cn

PHP:  array_merge(...$nested);
来源：http://cow.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ulk.ehwqpu.com

TS:   nested.flat();
来源：http://ehq.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kqh.bbcook.cn

Go:   // 手写双层循环
来源：http://yxw.ctjpmb.com

Ruby: nested.flatten
来源：http://nxs.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://gya.0kj1m.cn

[D19] 按字段分组
来源：http://skl.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pji.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ezy.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://amv.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ufz.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vis.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://xdp.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xrh.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jxt.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://bea.52xcode.cn

Py:   Counter(arr)
来源：http://sgq.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://qfb.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vko.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjn.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fqs.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://yfb.shuidangran.top

Ruby: arr.tally
来源：http://nct.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://obx.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://jau.chenzaomai.com

Py:   x in arr
来源：http://uvd.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://fyb.yuxming.cn

JS:   arr.includes(x)
来源：http://hdw.yj20258888.top

TS:   arr.includes(x)
来源：http://zag.gogol.net.cn

Java: list.contains(x)
来源：http://ong.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://etw.xuanzx.com

Ruby: arr.include?(x)
来源：http://tfd.meibo888.top

C#:   list.Contains(x)
来源：http://tpq.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://bya.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fud.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ayu.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xqq.andypj.xyz

TS:   [...arr];
来源：http://jpj.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://ehh.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://qyz.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://doe.jianghu66.top

C#:   new List<int>(list);
来源：http://yua.gaohongyu789.top

[D23] reduce 累积计算
来源：http://ubf.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://exc.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://inh.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hpp.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyv.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nta.pengpengdd.cyou

Go:   // 手写循环
来源：http://poo.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ljp.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eph.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://itv.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yij.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ndd.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uno.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uqf.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wkl.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzd.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zhd.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yhj.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://iwu.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fqi.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qhc.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lom.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xqu.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ncl.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nam.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://evl.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kci.zdqjudy.top

[D26] 数组转字符串
来源：http://ifb.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://iiq.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://yda.52xcode.cn

JS:   arr.join(", ")
来源：http://nqx.cqqwz.cn

TS:   arr.join(", ")
来源：http://ufy.wangdashe.top

Java: String.join(", ", list)
来源：http://mms.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://ytb.guowangkeji.top

Ruby: arr.join(", ")
来源：http://ggd.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://zqx.fengsongda.top

================================================================================
来源：http://ebs.bjfxy.top

E. 字符串处理
来源：http://oye.guannengcc.top

================================================================================
来源：http://xml.chenjidiqi.icu

[E01] 拼接字符串
来源：http://okn.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tmf.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ynv.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://shq.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dwu.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://svb.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://upw.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ord.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ech.zycfv.cn

[E02] 重复字符串
来源：http://ssl.ehwqpu.com

Py:   "ab" * 3
来源：http://ebx.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://hax.havefunace.top

JS:   "ab".repeat(3)
来源：http://hcf.fengsongda.top

TS:   "ab".repeat(3)
来源：http://chl.zdqjudy.top

Java: "ab".repeat(3)
来源：http://qii.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://rga.jianghu66.top

Ruby: "ab" * 3
来源：http://iox.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewm.daxiang520.top

[E03] 截取子串
来源：http://dfq.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zxu.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eyy.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gjy.pycfn.com

TS:   s.slice(1, 4)
来源：http://hyk.tian-w.cn

Java: s.substring(1, 4)
来源：http://huc.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vhu.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://cpf.meibo888.top

C#:   s.Substring(1, 3)
来源：http://eis.jlsjyb.cn

[E04] 查找子串位置
来源：http://yho.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://sfi.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://jnw.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://koc.bbcook.cn

TS:   s.indexOf("x")
来源：http://yra.kuanghao11.cn

Java: s.indexOf("x")
来源：http://cuf.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://osw.dianchejie.cn

Ruby: s.index("x")
来源：http://auo.sxryk.cn

C#:   s.IndexOf("x")
来源：http://dkw.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eti.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lwq.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xcy.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://roo.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tcx.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ein.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://onr.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zdz.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nax.kuanghao11.cn

[E06] 替换子串
来源：http://ama.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sep.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://rjq.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgi.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://hnb.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://svt.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kle.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://atb.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://ykv.0kj1m.cn

[E07] 按分隔符拆分
来源：http://sko.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://psk.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fcz.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hmj.guowangkeji.top

TS:   s.split(",")
来源：http://fgu.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://jru.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ito.yj202588.top

Ruby: s.split(",");  s.split
来源：http://ydv.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tyd.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://gsv.gotoacloud.top

Py:   ",".join(items)
来源：http://etn.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://mpe.tian-w.cn

JS:   items.join(",")
来源：http://zim.yvedp.cn

TS:   items.join(",")
来源：http://hrm.yj20258.top

Java: String.join(",", items)
来源：http://zry.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://coy.jqgfzy.top

Ruby: items.join(",")
来源：http://kkx.yfazqb.com

C#:   string.Join(",", items)
来源：http://qjq.jinqigufen.top

[E09] 去除所有空白字符
来源：http://kcz.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nnz.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kzi.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nko.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://rbd.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://xgq.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ppo.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://erg.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucl.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://hnb.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zcx.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hsn.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://rds.jiagoushi.top


<!-- 参考信息 -->