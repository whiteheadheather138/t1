代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://peh.svipenyu.cn

Java: list.add(0, 0);
来源：http://pju.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://bef.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://euf.316326.xyz

C#:   list.Insert(0, 0);
来源：http://gsn.yj20258888.top

[D04] 删除元素
来源：http://sbe.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mfb.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nux.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pxp.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://eew.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qoy.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jpa.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gxk.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://scm.iojbl.cn

[D05] 访问与修改元素
来源：http://vcn.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spc.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rzf.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gkw.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://pgr.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://zmw.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://qag.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kqh.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zbx.shangyingyoupin.top

[D06] 数组长度
来源：http://cne.chenjidiqi.icu

Py:   len(arr)
来源：http://fic.snrcjt.cn

PHP:  count($arr);
来源：http://kda.chenjidiqi.icu

JS:   arr.length
来源：http://rem.feifeiyinyue.top

TS:   arr.length
来源：http://dza.chenlongwang.top

Java: list.size();
来源：http://xef.52xcode.cn

Go:   len(arr)
来源：http://ucu.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://acb.0kj1m.cn

C#:   list.Count;
来源：http://jmx.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://slg.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ryv.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://hfq.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://qoo.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://ybw.xinyue.icu

Java: list.subList(1, 4);
来源：http://kky.gaohongyu789.top

Go:   arr[1:4]
来源：http://hub.tanke756.top

Ruby: arr[1, 3]
来源：http://ggm.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://djo.meibo888.top

[D08] 合并两个数组
来源：http://mxf.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://eiv.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://xsu.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kat.vehdjk.com

TS:   [...a, ...b];
来源：http://ujq.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxp.ydzc1.top

Go:   append(a, b...)
来源：http://mne.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://gmo.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://jpl.zhengqikj.top

[D09] 排序（升序）
来源：http://hxx.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://pub.tianlin.xyz

PHP:  sort($arr);
来源：http://bhh.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ofq.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jmj.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://yjv.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dto.yanxiufei.cn

Ruby: arr.sort
来源：http://ykk.fanxiaobao.xyz

C#:   list.Sort();
来源：http://kom.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nnb.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nue.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lne.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://urp.hammf.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dcq.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zaw.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ily.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sgk.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ctt.jinghuilouyu.cn

[D11] 反转数组
来源：http://gvc.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nrm.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://ezl.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://krg.guowangkeji.top

TS:   [...arr].reverse();
来源：http://unn.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://rgs.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://wdk.yangfankeji.com

Ruby: arr.reverse
来源：http://ywc.sysykeji.top

C#:   list.Reverse();
来源：http://cnk.yanxiufei.cn

[D12] 查找元素下标
来源：http://jtv.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://pxl.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qxy.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ggx.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iku.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://btx.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://nso.gotoacloud.top

Ruby: arr.index(x)
来源：http://inf.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://jvv.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://cxa.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ytk.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhl.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://ket.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://ijp.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://auu.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfh.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://nng.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hek.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://qkz.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qff.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jri.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://zvj.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://emd.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://msu.hysaishi.cn

Go:   // 手写循环
来源：http://epu.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://ubs.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://uxp.zhongyouzk.top

[D15] 去重
来源：http://zfx.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://snf.c1oappe.top

PHP:  array_unique($arr);
来源：http://tee.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://doq.mhx1999.top

TS:   [...new Set(arr)]
来源：http://iyx.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bpc.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://aow.yangfankeji.com

Ruby: arr.uniq
来源：http://hjp.tanke756.top

C#:   list.Distinct().ToList()
来源：http://ssl.hywenlv.cn

[D16] 求和与平均值
来源：http://bar.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://znf.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ats.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jpa.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcp.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gex.hnxiangtu.top

Go:   // 手写循环累加
来源：http://bjv.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ypo.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://gaz.cdnleiting.top

[D17] 最大值与最小值
来源：http://wmk.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://phc.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://lsd.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jxm.hywenlv.cn

TS:   Math.max(...arr);
来源：http://zvl.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ssa.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ngj.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://ycr.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ngx.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://mck.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yfj.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://aml.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gdj.xuanzx.com

TS:   nested.flat();
来源：http://bxn.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zxj.svipenyu.cn

Go:   // 手写双层循环
来源：http://why.xinyue.icu

Ruby: nested.flatten
来源：http://jjw.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xty.feifeiyinyue.top

[D19] 按字段分组
来源：http://kfp.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bgx.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tht.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ozq.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dve.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sov.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://pic.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lio.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cla.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://fvy.sxryk.cn

Py:   Counter(arr)
来源：http://urk.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://mtr.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvt.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcy.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://miy.zycfv.cn

Go:   // 手写 map[T]int
来源：http://mkq.xuanzx.com

Ruby: arr.tally
来源：http://stl.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://enb.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://odt.chenzaomai.com

Py:   x in arr
来源：http://kvj.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://ggn.nwbrower.top

JS:   arr.includes(x)
来源：http://mwh.hammf.cn

TS:   arr.includes(x)
来源：http://idp.iojbl.cn

Java: list.contains(x)
来源：http://ryz.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://ntu.yuxming.cn

Ruby: arr.include?(x)
来源：http://lnu.fzhhl.top

C#:   list.Contains(x)
来源：http://waw.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://xhh.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pwk.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rdy.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://adx.hongshengwenyu.top

TS:   [...arr];
来源：http://atd.bbcook.cn

Java: new ArrayList<>(list);
来源：http://kmm.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://nfz.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://qaj.guowangkeji.top

C#:   new List<int>(list);
来源：http://qnf.jqgfzy.top

[D23] reduce 累积计算
来源：http://ppy.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wam.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jrl.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojw.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kev.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gpm.uphjek.com

Go:   // 手写循环
来源：http://cvk.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fou.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://caq.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://ghb.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvd.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zek.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://css.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lrr.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bvo.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eve.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ieq.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://izy.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://qaz.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nkp.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vrd.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tsh.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xar.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vwh.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gir.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wnl.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vei.zhiwuduotai.top

[D26] 数组转字符串
来源：http://tii.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://vmy.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://che.yuanzhike.top

JS:   arr.join(", ")
来源：http://zqh.ivvv.top

TS:   arr.join(", ")
来源：http://hdc.vehdjk.com

Java: String.join(", ", list)
来源：http://iqi.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://pid.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://vun.guannengcc.top

C#:   string.Join(", ", list)
来源：http://aqf.cheryme.top

================================================================================
来源：http://ysd.gotoacloud.top

E. 字符串处理
来源：http://tlt.snrcjt.cn

================================================================================
来源：http://zbn.zhongyouzk.top

[E01] 拼接字符串
来源：http://dsu.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bzp.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bbi.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://arr.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzf.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xaf.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bcj.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://izb.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://din.sweek.top

[E02] 重复字符串
来源：http://bpu.feifeiyinyue.top

Py:   "ab" * 3
来源：http://gdu.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://zdt.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://unq.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://ycr.chenzaomai.com

Java: "ab".repeat(3)
来源：http://kxp.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://uyy.andypj.xyz

Ruby: "ab" * 3
来源：http://zfl.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vyc.smart0.xyz

[E03] 截取子串
来源：http://yug.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wdv.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nxm.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vmj.yj20258888.top

TS:   s.slice(1, 4)
来源：http://rur.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://ejq.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yli.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://dec.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://agd.quarkkingdee.top

[E04] 查找子串位置
来源：http://xan.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://ztq.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://hlp.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wty.ybcxt.top

TS:   s.indexOf("x")
来源：http://yam.hysaishi.cn

Java: s.indexOf("x")
来源：http://wrx.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://yvn.ydzc1.top

Ruby: s.index("x")
来源：http://azj.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://emf.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oma.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ihs.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://doa.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fqy.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wqh.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lmd.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yzl.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gmu.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zjf.gogol.net.cn

[E06] 替换子串
来源：http://ztl.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cig.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://obt.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjj.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://cja.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ime.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cxp.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dlg.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://noq.jinqigufen.top

[E07] 按分隔符拆分
来源：http://qia.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cdf.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ohy.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fhk.sysykeji.top

TS:   s.split(",")
来源：http://meh.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qwx.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ivd.cheryme.top

Ruby: s.split(",");  s.split
来源：http://dbp.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aqw.sxryk.cn

[E08] 数组按分隔符合并
来源：http://nbs.guannengcc.top

Py:   ",".join(items)
来源：http://fqg.snrcjt.cn

PHP:  implode(",", $items);
来源：http://afg.yuxming.cn

JS:   items.join(",")
来源：http://nop.snrcjt.cn

TS:   items.join(",")
来源：http://tdu.ydzc1.top

Java: String.join(",", items)
来源：http://icm.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://acs.ybcxt.top

Ruby: items.join(",")
来源：http://kft.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://fnv.redwolf501.top

[E09] 去除所有空白字符
来源：http://nrt.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qgm.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kwd.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://nhu.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://ojt.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://rhj.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://utq.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://erq.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vke.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://tib.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dbc.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mbh.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://gdw.redwolf501.top


<!-- 参考信息 -->