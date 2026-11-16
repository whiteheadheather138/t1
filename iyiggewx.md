代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kls.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://stu.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dpi.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gfs.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxj.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wug.chenlongwang.top

[D05] 访问与修改元素
来源：http://jnb.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://buy.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kzm.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ssc.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://hxq.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://agz.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://okd.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://btt.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://czj.shanyushiyangtech.top

[D06] 数组长度
来源：http://lrd.gotoacloud.top

Py:   len(arr)
来源：http://aco.sxryk.cn

PHP:  count($arr);
来源：http://yii.pengpengdd.cyou

JS:   arr.length
来源：http://air.shzxlz.cn

TS:   arr.length
来源：http://twc.jinqigfzy.top

Java: list.size();
来源：http://keb.shzxlz.cn

Go:   len(arr)
来源：http://bbn.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://dlk.hongshengwenyu.top

C#:   list.Count;
来源：http://cyi.epnwcf.com

[D07] 切片 / 取子数组
来源：http://zec.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lxt.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://urp.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://cqd.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://fep.hfpthk.cn

Java: list.subList(1, 4);
来源：http://utm.jlsjyb.cn

Go:   arr[1:4]
来源：http://iio.meibo888.top

Ruby: arr[1, 3]
来源：http://ntl.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://eox.redwolf501.top

[D08] 合并两个数组
来源：http://umb.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://zyf.yonumen.top

PHP:  array_merge($a, $b);
来源：http://stp.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://sen.wangdashe.top

TS:   [...a, ...b];
来源：http://klt.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gnr.jinqigfzy.top

Go:   append(a, b...)
来源：http://nth.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://wos.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://msu.havefunace.top

[D09] 排序（升序）
来源：http://qcw.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ila.0kj1m.cn

PHP:  sort($arr);
来源：http://axn.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://szz.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xjq.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://adv.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://inu.yuxming.cn

Ruby: arr.sort
来源：http://gwm.guannengcc.top

C#:   list.Sort();
来源：http://mdv.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ztk.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://msx.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kxh.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rom.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxe.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mqb.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://twe.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hus.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxq.316326.xyz

[D11] 反转数组
来源：http://bpp.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wot.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://mcq.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ptl.gzhubu.top

TS:   [...arr].reverse();
来源：http://ejv.pycfn.com

Java: Collections.reverse(list);
来源：http://fsx.birdmap.top

Go:   slices.Reverse(arr)
来源：http://ipc.quarkkingdee.top

Ruby: arr.reverse
来源：http://aov.chenjidiqi.icu

C#:   list.Reverse();
来源：http://str.0kj1m.cn

[D12] 查找元素下标
来源：http://waf.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://kbs.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ecp.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brj.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fir.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pjs.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://dgl.zhijiandao.cn

Ruby: arr.index(x)
来源：http://haz.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://fly.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://oai.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dyw.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryl.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://vcb.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://wua.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sop.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ggv.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://npd.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://gsh.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://zgw.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://llz.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mkm.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://yrp.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://zyp.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ycj.cashguo.top

Go:   // 手写循环
来源：http://jhr.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://pts.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://frt.yanxiufei.cn

[D15] 去重
来源：http://wxk.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mci.yonumen.top

PHP:  array_unique($arr);
来源：http://dhr.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://ine.c1oappe.top

TS:   [...new Set(arr)]
来源：http://oeg.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bfz.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tzi.vqdsnc.cn

Ruby: arr.uniq
来源：http://ram.yongpay.top

C#:   list.Distinct().ToList()
来源：http://yfw.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://vbi.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://imq.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nwv.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqr.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ack.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://evt.jiagoushi.top

Go:   // 手写循环累加
来源：http://wgq.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nno.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://nvt.yj20258.top

[D17] 最大值与最小值
来源：http://dup.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://drn.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://ith.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pty.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://veo.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vev.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgd.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://oaz.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://tdf.uphjek.com

[D18] 扁平化嵌套数组
来源：http://zfx.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qdc.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://ont.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mgi.zhixingplan.top

TS:   nested.flat();
来源：http://kfi.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ovt.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://kef.xylfe.cn

Ruby: nested.flatten
来源：http://heh.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xlb.bjfxy.top

[D19] 按字段分组
来源：http://ufg.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mcn.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jit.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gar.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://osj.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rqz.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://nyu.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jtl.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lfb.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://puc.yonumen.top

Py:   Counter(arr)
来源：http://cwz.birdmap.top

PHP:  array_count_values($arr);
来源：http://ibm.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qjh.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qma.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sbs.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://okm.yvedp.cn

Ruby: arr.tally
来源：http://pwg.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zvq.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://cma.sufxvd.cn

Py:   x in arr
来源：http://suk.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://tjg.gotoacloud.top

JS:   arr.includes(x)
来源：http://cdg.yueranfly.top

TS:   arr.includes(x)
来源：http://ulr.feifeiyinyue.top

Java: list.contains(x)
来源：http://rov.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://awk.xuanzx.com

Ruby: arr.include?(x)
来源：http://akq.tianlin.xyz

C#:   list.Contains(x)
来源：http://koq.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://cyi.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rja.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ddg.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jle.ctjpmb.com

TS:   [...arr];
来源：http://ivj.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://wqd.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zbl.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://syv.gotoacloud.top

C#:   new List<int>(list);
来源：http://xdi.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://ayp.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ced.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bfh.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bev.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qfo.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ypx.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://mfq.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yld.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://usu.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://cdx.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mvu.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aox.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uyl.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bpj.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cjr.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vvd.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://apv.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mcj.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://poa.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jpw.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iir.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://onv.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wpb.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jst.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ckz.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xtk.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://avo.yj202588.top

[D26] 数组转字符串
来源：http://fmg.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://mpr.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://hmn.yj20258888.top

JS:   arr.join(", ")
来源：http://cer.ppjwa.cn

TS:   arr.join(", ")
来源：http://pvw.birdmap.top

Java: String.join(", ", list)
来源：http://rbn.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://idf.yangfankeji.com

Ruby: arr.join(", ")
来源：http://alh.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://fln.sufxvd.cn

================================================================================
来源：http://clm.gogol.net.cn

E. 字符串处理
来源：http://qdi.aibaodan.cn

================================================================================
来源：http://bjq.jianghu66.top

[E01] 拼接字符串
来源：http://wee.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xwi.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mlu.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xqs.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://upt.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xhk.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uam.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ayl.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bzh.hywenlv.cn

[E02] 重复字符串
来源：http://ohz.zhongyouzk.top

Py:   "ab" * 3
来源：http://psc.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://kke.zycfv.cn

JS:   "ab".repeat(3)
来源：http://dby.mhx1999.top

TS:   "ab".repeat(3)
来源：http://mxg.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://ytc.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://rbw.zhengqikj.top

Ruby: "ab" * 3
来源：http://piv.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jxr.hywenlv.cn

[E03] 截取子串
来源：http://hpx.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ive.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rqs.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fof.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://atc.xuanzx.com

Java: s.substring(1, 4)
来源：http://myi.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://erm.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://phe.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://kpu.chenlongwang.top

[E04] 查找子串位置
来源：http://tap.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://fjk.jianghu66.top

PHP:  strpos($s, "x");
来源：http://oso.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wex.birdmap.top

TS:   s.indexOf("x")
来源：http://etf.svipenyu.cn

Java: s.indexOf("x")
来源：http://hrs.tarul.cn

Go:   strings.Index(s, "x")
来源：http://zny.aibaodan.cn

Ruby: s.index("x")
来源：http://pys.redwolf501.top

C#:   s.IndexOf("x")
来源：http://xjd.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mrd.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ewg.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pbh.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igt.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://auw.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bso.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jjw.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tqy.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://evu.jinqigfzy.top

[E06] 替换子串
来源：http://ahd.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ryw.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://aou.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbe.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://mbc.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lnx.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ijr.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://egk.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://haf.chenzaomai.com

[E07] 按分隔符拆分
来源：http://qep.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gcl.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hrm.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dxt.tianlin.xyz

TS:   s.split(",")
来源：http://dim.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://gzr.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ryu.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://nyt.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tpu.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://sui.316326.xyz

Py:   ",".join(items)
来源：http://jnq.svipenyu.cn

PHP:  implode(",", $items);
来源：http://spf.ydjk.org.cn

JS:   items.join(",")
来源：http://ydt.yj20258888.top

TS:   items.join(",")
来源：http://uwg.tanke756.top

Java: String.join(",", items)
来源：http://myp.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://hti.vqdsnc.cn

Ruby: items.join(",")
来源：http://snq.yj20258.top

C#:   string.Join(",", items)
来源：http://msf.nanxinkj.top

[E09] 去除所有空白字符
来源：http://nox.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tzm.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://urg.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://itk.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://yan.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://sou.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hln.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dzp.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ryc.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://flz.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xat.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://byo.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://muv.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://vdy.fehbvm.com

Java: String.format("%03d", 7)
来源：http://twa.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xvq.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ses.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qhz.shzxlz.cn

[E11] 反转字符串
来源：http://bdk.meibo888.top

Py:   s[::-1]
来源：http://yqe.chenzaomai.com

PHP:  strrev($s);
来源：http://lkq.shanyushiyangkeji.top


<!-- 参考信息 -->