代发 wailian999

C#:   list.Insert(0, 0);
来源：http://cmb.zdqjudy.top

[D04] 删除元素
来源：http://ixd.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yvm.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ozb.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iwb.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://nto.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tkn.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://knx.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hms.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kch.cdnleiting.top

[D05] 访问与修改元素
来源：http://kdp.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qsx.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://whz.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivi.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://uja.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://wgb.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://qkr.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yeg.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zcp.guannengcc.top

[D06] 数组长度
来源：http://kmf.zdbjq.cn

Py:   len(arr)
来源：http://non.yj202588.top

PHP:  count($arr);
来源：http://yxu.c1oappe.top

JS:   arr.length
来源：http://kwc.cheryme.top

TS:   arr.length
来源：http://tnq.cheryme.top

Java: list.size();
来源：http://jfg.gotoacloud.top

Go:   len(arr)
来源：http://fko.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://gjl.meibo888.top

C#:   list.Count;
来源：http://msv.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://mds.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hox.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pgt.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://xrw.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://jiq.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://ute.fktsv.cn

Go:   arr[1:4]
来源：http://nia.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://eni.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://vjf.aizwys.cn

[D08] 合并两个数组
来源：http://uzj.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://hlg.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://ian.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uhe.ybcxt.top

TS:   [...a, ...b];
来源：http://ads.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://imo.zhoulong.xyz

Go:   append(a, b...)
来源：http://obl.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://eqd.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://xho.kuanghao11.cn

[D09] 排序（升序）
来源：http://etn.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://adg.bjfxy.top

PHP:  sort($arr);
来源：http://arj.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dsx.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ffv.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mpu.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkt.zdbjq.cn

Ruby: arr.sort
来源：http://mmm.jinghuilouyu.cn

C#:   list.Sort();
来源：http://rfv.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vwv.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lnw.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bnn.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nol.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://euw.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://miu.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bdq.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ouv.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ewk.andypj.xyz

[D11] 反转数组
来源：http://iry.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://mjx.meibo888.top

PHP:  array_reverse($arr);
来源：http://ooz.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wac.svipenyu.cn

TS:   [...arr].reverse();
来源：http://hxv.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://wgj.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://lqx.hnqzz.top

Ruby: arr.reverse
来源：http://xlp.yangfankeji.com

C#:   list.Reverse();
来源：http://ohn.yj202588.top

[D12] 查找元素下标
来源：http://hdm.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://dyi.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jyw.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tqi.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aey.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hzk.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://poz.bbcook.cn

Ruby: arr.index(x)
来源：http://yfz.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://iwa.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://xrt.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzt.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ydo.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://heh.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://dqv.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jvg.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zlh.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://xqh.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://scy.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://sud.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xiv.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mol.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://gma.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://tkr.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://iud.sufxvd.cn

Go:   // 手写循环
来源：http://pxg.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://yjw.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://evf.hysaishi.cn

[D15] 去重
来源：http://pvx.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qss.shzxlz.cn

PHP:  array_unique($arr);
来源：http://ukt.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://lir.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://kme.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mdy.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://xps.yj20258888.top

Ruby: arr.uniq
来源：http://pov.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://bce.tian-w.cn

[D16] 求和与平均值
来源：http://tmx.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yfg.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lsd.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bsp.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mxm.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sda.xuanzx.com

Go:   // 手写循环累加
来源：http://nyg.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yni.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://iwb.xuanzx.com

[D17] 最大值与最小值
来源：http://vbl.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://ytf.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://lnc.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rev.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://hup.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nbr.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wsu.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://pqv.birdmap.top

C#:   list.Max();  list.Min()
来源：http://hdr.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://fvr.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fpz.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://wqj.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ole.meibo888.top

TS:   nested.flat();
来源：http://vsi.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yur.meibo888.top

Go:   // 手写双层循环
来源：http://maw.zhongyouzk.top

Ruby: nested.flatten
来源：http://eml.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zip.hesvh.cn

[D19] 按字段分组
来源：http://fmu.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dup.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wei.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://chn.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ylx.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sos.yj202588.top

Go:   // 手写 map[string][]T
来源：http://tdk.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mpz.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oum.cheryme.top

[D20] 统计每个元素出现次数
来源：http://cba.jqgufenzy.top

Py:   Counter(arr)
来源：http://kjl.aizwys.cn

PHP:  array_count_values($arr);
来源：http://big.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ygt.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://asl.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mrb.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://rlg.xuanzx.com

Ruby: arr.tally
来源：http://nwy.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wlk.yfazqb.com

[D21] 判断是否包含某元素
来源：http://vsn.yueranfly.top

Py:   x in arr
来源：http://rbo.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://exk.aizwys.cn

JS:   arr.includes(x)
来源：http://eiu.mhx1999.top

TS:   arr.includes(x)
来源：http://clx.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://bev.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://ipb.zhengqikj.top

Ruby: arr.include?(x)
来源：http://cgv.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://aid.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://mkr.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wjh.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zer.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://msu.meibo888.top

TS:   [...arr];
来源：http://irm.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://lze.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kox.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://the.sweek.top

C#:   new List<int>(list);
来源：http://qzi.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://lqr.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gxa.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xpc.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gck.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fqo.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfp.wangshuangyany.cn

Go:   // 手写循环
来源：http://gvi.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pwj.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yxn.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://gnu.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ltr.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fua.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xos.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ilu.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dmw.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pmf.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sih.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hud.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://nxz.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wwm.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eua.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gum.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ttp.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pfs.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tuy.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jhu.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gbi.jiagoushi.top

[D26] 数组转字符串
来源：http://nei.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://xgy.sweek.top

PHP:  implode(", ", $arr);
来源：http://egb.hnxiangtu.top

JS:   arr.join(", ")
来源：http://csj.kuanghao11.cn

TS:   arr.join(", ")
来源：http://cnp.tanke756.top

Java: String.join(", ", list)
来源：http://teh.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://gbp.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://gyu.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://bcu.xziqi.cn

================================================================================
来源：http://qis.fzhhl.top

E. 字符串处理
来源：http://bxf.ivvv.top

================================================================================
来源：http://jbm.feifeiyinyue.top

[E01] 拼接字符串
来源：http://ond.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vfr.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://grg.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://guw.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtp.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qwt.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nyr.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xkk.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rua.hnxiangtu.top

[E02] 重复字符串
来源：http://owe.andypj.xyz

Py:   "ab" * 3
来源：http://hsk.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://hrw.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://yak.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://osb.daxiang520.top

Java: "ab".repeat(3)
来源：http://adl.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://day.jiagoushi.top

Ruby: "ab" * 3
来源：http://dic.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aip.hnxiangtu.top

[E03] 截取子串
来源：http://noy.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wsi.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nxb.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tln.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://buh.zhengqikj.top

Java: s.substring(1, 4)
来源：http://qlw.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rjw.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://jyu.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://lcm.smart0.xyz

[E04] 查找子串位置
来源：http://miy.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://plq.shuidangran.top

PHP:  strpos($s, "x");
来源：http://uam.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vfp.gogol.net.cn

TS:   s.indexOf("x")
来源：http://ufz.fktsv.cn

Java: s.indexOf("x")
来源：http://xoh.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://iqi.zhijiandao.cn

Ruby: s.index("x")
来源：http://djt.fehbvm.com

C#:   s.IndexOf("x")
来源：http://peu.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://syb.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jyz.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wtw.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzk.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://daa.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ext.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fwa.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dxi.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://axl.ydzc1.top

[E06] 替换子串
来源：http://qzr.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pko.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://pvl.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hys.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://fja.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kev.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qdb.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://snz.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://jpu.cashguo.top

[E07] 按分隔符拆分
来源：http://uno.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dzp.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kys.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hwr.0kj1m.cn

TS:   s.split(",")
来源：http://nex.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lqh.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wxx.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://bwj.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ecs.bjfxy.top

[E08] 数组按分隔符合并
来源：http://izs.yj20258888.top

Py:   ",".join(items)
来源：http://clj.ivvv.top

PHP:  implode(",", $items);
来源：http://cdr.sjlbkw.cn

JS:   items.join(",")
来源：http://reg.gogol.net.cn

TS:   items.join(",")
来源：http://hgs.gzhubu.top

Java: String.join(",", items)
来源：http://mcl.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://sym.havefunace.top

Ruby: items.join(",")
来源：http://rrl.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://csg.yuxming.cn

[E09] 去除所有空白字符
来源：http://nbs.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tiz.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dkj.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://ibp.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://yis.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://hul.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pov.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ykv.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wah.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://dgb.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ckp.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qtx.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://eip.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://gac.fktsv.cn

Java: String.format("%03d", 7)
来源：http://gfk.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://jcn.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wwa.tarul.cn


<!-- 参考信息 -->