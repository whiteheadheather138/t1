代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://udy.xziqi.cn

Java: list.add(0, 0);
来源：http://wef.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cln.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tvg.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://qiv.cdnleiting.top

[D04] 删除元素
来源：http://zir.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gmi.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jkv.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ozi.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://sda.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rqo.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://khn.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqa.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ups.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://vme.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bgh.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lmz.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ysh.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://mhu.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://wvw.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://grn.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfl.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dpe.guowangkeji.top

[D06] 数组长度
来源：http://cjo.yueranfly.top

Py:   len(arr)
来源：http://ggu.chenzaomai.com

PHP:  count($arr);
来源：http://zbh.quarkkingdee.top

JS:   arr.length
来源：http://pbp.tanke756.top

TS:   arr.length
来源：http://lfs.snrcjt.cn

Java: list.size();
来源：http://qov.hammf.cn

Go:   len(arr)
来源：http://uix.fktsv.cn

Ruby: arr.length; arr.size
来源：http://qbg.hnqzz.top

C#:   list.Count;
来源：http://kjh.yvedp.cn

[D07] 切片 / 取子数组
来源：http://ufw.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rth.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://huq.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://ppg.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://cjn.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://rro.yj20258888.top

Go:   arr[1:4]
来源：http://ufo.zycfv.cn

Ruby: arr[1, 3]
来源：http://ixz.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://vre.ppjwa.cn

[D08] 合并两个数组
来源：http://riy.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://tgh.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://gtx.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://osv.zhixingplan.top

TS:   [...a, ...b];
来源：http://jts.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qzr.yj202588.top

Go:   append(a, b...)
来源：http://szw.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://lrq.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://ydd.hysaishi.cn

[D09] 排序（升序）
来源：http://jts.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://wgk.hnqzz.top

PHP:  sort($arr);
来源：http://zyk.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vfy.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywh.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://xqa.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmo.vqdsnc.cn

Ruby: arr.sort
来源：http://srw.epnwcf.com

C#:   list.Sort();
来源：http://gzm.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pkt.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mrr.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwi.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvn.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gmc.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pnq.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cmv.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sgd.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rzw.52xcode.cn

[D11] 反转数组
来源：http://wtk.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://hda.sysykeji.top

PHP:  array_reverse($arr);
来源：http://dcr.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qen.chenzaomai.com

TS:   [...arr].reverse();
来源：http://dvf.smart0.xyz

Java: Collections.reverse(list);
来源：http://xad.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://rfo.chenzaomai.com

Ruby: arr.reverse
来源：http://tdq.ydzc1.top

C#:   list.Reverse();
来源：http://uzt.jinqigufen.top

[D12] 查找元素下标
来源：http://thm.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://iaj.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oxg.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgw.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxu.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nbj.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://lgx.nwbrower.top

Ruby: arr.index(x)
来源：http://yjf.hnqzz.top

C#:   list.IndexOf(x);
来源：http://vic.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://ggl.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rfb.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jpw.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://boj.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://yrj.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rgl.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugn.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dco.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bef.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://nfm.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://slx.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zcv.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://eoa.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://ehn.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ypo.ivvv.top

Go:   // 手写循环
来源：http://uyi.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mtp.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://fya.birdmap.top

[D15] 去重
来源：http://yre.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cyy.cashguo.top

PHP:  array_unique($arr);
来源：http://cte.hammf.cn

JS:   [...new Set(arr)]
来源：http://vwk.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://olz.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://one.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://szo.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://twb.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://sec.cqqwz.cn

[D16] 求和与平均值
来源：http://esk.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pep.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sub.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sap.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iry.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ush.shuidangran.top

Go:   // 手写循环累加
来源：http://cio.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tyj.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://xiq.sxryk.cn

[D17] 最大值与最小值
来源：http://luq.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://snv.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://hvu.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kty.ydzc1.top

TS:   Math.max(...arr);
来源：http://nlf.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oxs.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tba.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://dhj.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://wab.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://mtp.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://asc.meibo888.top

PHP:  array_merge(...$nested);
来源：http://sdf.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owp.kuanghao11.cn

TS:   nested.flat();
来源：http://pnf.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uwo.uphjek.com

Go:   // 手写双层循环
来源：http://xzd.cqqwz.cn

Ruby: nested.flatten
来源：http://xlj.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://eds.gzhubu.top

[D19] 按字段分组
来源：http://hmq.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fce.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oxx.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hde.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hwp.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vxr.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://ind.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fum.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lhw.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://ety.ppjwa.cn

Py:   Counter(arr)
来源：http://pwu.cheryme.top

PHP:  array_count_values($arr);
来源：http://rvu.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://egd.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lwx.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iqq.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://wyw.jlsjyb.cn

Ruby: arr.tally
来源：http://jbo.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xhc.epnwcf.com

[D21] 判断是否包含某元素
来源：http://fzy.fanxiaobao.xyz

Py:   x in arr
来源：http://qlp.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://oeh.andypj.xyz

JS:   arr.includes(x)
来源：http://ipo.hysaishi.cn

TS:   arr.includes(x)
来源：http://jmv.haohaochexian.top

Java: list.contains(x)
来源：http://ifh.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://mjb.yfazqb.com

Ruby: arr.include?(x)
来源：http://npx.9152youxi.cn

C#:   list.Contains(x)
来源：http://uad.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://pfv.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ygf.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yiy.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://swk.sjlbkw.cn

TS:   [...arr];
来源：http://yzp.fehbvm.com

Java: new ArrayList<>(list);
来源：http://zte.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://nkd.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://fsj.wangdashe.top

C#:   new List<int>(list);
来源：http://zce.sufxvd.cn

[D23] reduce 累积计算
来源：http://npj.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cgk.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tko.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzy.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kuv.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gmi.jiagoushi.top

Go:   // 手写循环
来源：http://zpl.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hcw.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zzi.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://vfa.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iwd.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvm.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://inm.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pxg.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://por.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jsm.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xct.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kpc.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://igw.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ukx.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eet.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hbt.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tij.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xkc.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://crc.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qgs.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://amw.iojbl.cn

[D26] 数组转字符串
来源：http://hgh.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://kwr.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://nam.jiagoushi.top

JS:   arr.join(", ")
来源：http://qlv.xylfe.cn

TS:   arr.join(", ")
来源：http://mbh.yj20258888.top

Java: String.join(", ", list)
来源：http://sms.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://prm.nanxinkj.top

Ruby: arr.join(", ")
来源：http://cwj.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://wkt.chenjidiqi.icu

================================================================================
来源：http://mdr.c1oappe.top

E. 字符串处理
来源：http://mht.yuxming.cn

================================================================================
来源：http://kbt.yvedp.cn

[E01] 拼接字符串
来源：http://ujn.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kfk.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://omf.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hux.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jpm.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vuc.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oju.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://suv.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rtm.wangshuangyany.cn

[E02] 重复字符串
来源：http://vjb.tianlin.xyz

Py:   "ab" * 3
来源：http://baa.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://ozw.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://thh.gzhubu.top

TS:   "ab".repeat(3)
来源：http://ytq.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://wku.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://nrx.birdmap.top

Ruby: "ab" * 3
来源：http://jdo.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://isc.hesvh.cn

[E03] 截取子串
来源：http://msc.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oko.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ryq.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hup.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://uko.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://crz.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zjb.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ego.cashguo.top

C#:   s.Substring(1, 3)
来源：http://msx.shzxlz.cn

[E04] 查找子串位置
来源：http://uuv.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://rwg.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://ghe.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zvd.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://vmn.haohaochexian.top

Java: s.indexOf("x")
来源：http://lyx.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://kef.fengsongda.top

Ruby: s.index("x")
来源：http://leh.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://ydj.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jvs.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xvn.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tkw.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucy.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qpx.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ynk.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gif.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://plc.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uzz.sxryk.cn

[E06] 替换子串
来源：http://uyo.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vgi.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://wwx.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xif.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://ncn.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bci.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qdx.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gzb.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://nsw.iojbl.cn

[E07] 按分隔符拆分
来源：http://awj.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pgn.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mws.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tjs.ehwqpu.com

TS:   s.split(",")
来源：http://cpu.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://sea.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sdm.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://hme.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tac.fzhhl.top

[E08] 数组按分隔符合并
来源：http://why.tian-w.cn

Py:   ",".join(items)
来源：http://wyl.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://yss.vehdjk.com

JS:   items.join(",")
来源：http://ine.hcnkem.com

TS:   items.join(",")
来源：http://web.birdmap.top

Java: String.join(",", items)
来源：http://hpy.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://ltm.xuanzx.com

Ruby: items.join(",")
来源：http://luw.fehbvm.com

C#:   string.Join(",", items)
来源：http://wyj.ybcxt.top

[E09] 去除所有空白字符
来源：http://rlh.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ksr.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wag.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://gvh.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://zcq.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://pas.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fko.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://fzu.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lps.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://nod.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mnj.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xys.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://hom.yueranfly.top


<!-- 参考信息 -->