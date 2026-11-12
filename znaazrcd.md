代发 wailian999

Java: list.size();
来源：http://xjj.zhiwuduotai.top

Go:   len(arr)
来源：http://nvd.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://drq.gogol.net.cn

C#:   list.Count;
来源：http://wee.redwolf501.top

[D07] 切片 / 取子数组
来源：http://xbe.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nwd.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://mpg.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://irw.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://ljk.xziqi.cn

Java: list.subList(1, 4);
来源：http://rlj.hnqzz.top

Go:   arr[1:4]
来源：http://buj.dianchejie.cn

Ruby: arr[1, 3]
来源：http://zkk.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://zwt.pycfn.com

[D08] 合并两个数组
来源：http://bwq.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://kfl.pycfn.com

PHP:  array_merge($a, $b);
来源：http://lpm.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rwm.svipenyu.cn

TS:   [...a, ...b];
来源：http://mxz.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hvp.jqgfzy.top

Go:   append(a, b...)
来源：http://ilq.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://msx.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://lun.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://kuq.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://spr.feifeiyinyue.top

PHP:  sort($arr);
来源：http://tdn.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ssp.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://qbm.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://btp.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qby.jlsjyb.cn

Ruby: arr.sort
来源：http://ptn.aizwys.cn

C#:   list.Sort();
来源：http://hmy.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dgr.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ldz.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rml.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ade.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rmn.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mvs.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xnt.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jec.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://onp.zhaomingkeji.xyz

[D11] 反转数组
来源：http://zis.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://lan.bbcook.cn

PHP:  array_reverse($arr);
来源：http://kga.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vvj.cashguo.top

TS:   [...arr].reverse();
来源：http://byl.shzxlz.cn

Java: Collections.reverse(list);
来源：http://rhk.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://lyp.zycfv.cn

Ruby: arr.reverse
来源：http://fod.yueranfly.top

C#:   list.Reverse();
来源：http://qrn.pycfn.com

[D12] 查找元素下标
来源：http://aqc.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://rpe.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rez.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wuj.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqw.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bby.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://ugt.ppjwa.cn

Ruby: arr.index(x)
来源：http://imv.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://stz.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://iwc.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hgp.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://laa.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://bws.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://ozm.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrf.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://btr.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://evy.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xyd.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://fhh.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mbn.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tdw.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://tjb.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://uqp.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://whf.vqdsnc.cn

Go:   // 手写循环
来源：http://pjs.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://oxp.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pjl.hysaishi.cn

[D15] 去重
来源：http://efz.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgj.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://frc.sysykeji.top

JS:   [...new Set(arr)]
来源：http://fee.daria6918.cn

TS:   [...new Set(arr)]
来源：http://sxr.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vmi.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://jcy.xziqi.cn

Ruby: arr.uniq
来源：http://mrw.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://tec.ppjwa.cn

[D16] 求和与平均值
来源：http://ryz.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wgj.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vea.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfp.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgw.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kcw.yanxiufei.cn

Go:   // 手写循环累加
来源：http://udx.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rxk.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://mkx.cqqwz.cn

[D17] 最大值与最小值
来源：http://nov.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://osx.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://yfd.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tht.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://lcb.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zgp.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fkb.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://frg.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://lcp.pycfn.com

[D18] 扁平化嵌套数组
来源：http://arf.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibc.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://owu.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pgj.yueranfly.top

TS:   nested.flat();
来源：http://kus.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bqs.gaohongyu789.top

Go:   // 手写双层循环
来源：http://qvs.xinyue.icu

Ruby: nested.flatten
来源：http://ukr.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nfb.shangyingyoupin.top

[D19] 按字段分组
来源：http://cts.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bmz.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pai.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://voy.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vis.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzq.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://ghe.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqk.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ssp.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://diy.ivvv.top

Py:   Counter(arr)
来源：http://yfu.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://xnp.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zks.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uxl.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xnq.vehdjk.com

Go:   // 手写 map[T]int
来源：http://ccz.zhongyouzk.top

Ruby: arr.tally
来源：http://oko.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ctx.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://pzt.ivvv.top

Py:   x in arr
来源：http://wei.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://kya.smart0.xyz

JS:   arr.includes(x)
来源：http://lef.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://nzo.svipenyu.cn

Java: list.contains(x)
来源：http://swq.sweek.top

Go:   slices.Contains(arr, x)
来源：http://tjx.yuxming.cn

Ruby: arr.include?(x)
来源：http://qmh.52xcode.cn

C#:   list.Contains(x)
来源：http://hwq.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://jco.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ccl.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hlk.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ykn.zhongyouzk.top

TS:   [...arr];
来源：http://ihj.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://hbs.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yfh.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://ykh.kuanghao11.cn

C#:   new List<int>(list);
来源：http://uhq.yuxming.cn

[D23] reduce 累积计算
来源：http://egb.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zca.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lkd.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxh.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://etw.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://apu.guowangkeji.top

Go:   // 手写循环
来源：http://usz.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wbm.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mco.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://peb.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://obc.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvk.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jlt.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ztm.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kek.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sff.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jvt.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vco.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://fiq.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zcw.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cet.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rxp.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hzh.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pfb.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nbc.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ohi.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://skv.sxryk.cn

[D26] 数组转字符串
来源：http://gkp.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://jos.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://qci.pycfn.com

JS:   arr.join(", ")
来源：http://ssb.ybcxt.top

TS:   arr.join(", ")
来源：http://stw.yuxming.cn

Java: String.join(", ", list)
来源：http://isw.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://cja.yuanzhike.top

Ruby: arr.join(", ")
来源：http://oeg.yj20258.top

C#:   string.Join(", ", list)
来源：http://sgj.zhijiandao.cn

================================================================================
来源：http://nig.52xcode.cn

E. 字符串处理
来源：http://ihn.shzxlz.cn

================================================================================
来源：http://qgc.zdqjudy.top

[E01] 拼接字符串
来源：http://tdd.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lzo.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mvp.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxw.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://syq.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ksp.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mzm.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://okp.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lzb.sufxvd.cn

[E02] 重复字符串
来源：http://nvh.cheryme.top

Py:   "ab" * 3
来源：http://sjg.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://zoe.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://iup.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://vwq.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://czg.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://wqy.yfazqb.com

Ruby: "ab" * 3
来源：http://zca.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eeg.jinghuilouyu.cn

[E03] 截取子串
来源：http://jqd.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://snp.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ltj.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rnw.xuanzx.com

TS:   s.slice(1, 4)
来源：http://vmm.ybcxt.top

Java: s.substring(1, 4)
来源：http://ysl.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://syr.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://fic.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://hda.quarkkingdee.top

[E04] 查找子串位置
来源：http://dnl.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://xtr.fzhhl.top

PHP:  strpos($s, "x");
来源：http://cbx.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zkn.ctjpmb.com

TS:   s.indexOf("x")
来源：http://wvz.tarul.cn

Java: s.indexOf("x")
来源：http://qsk.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://dvd.epnwcf.com

Ruby: s.index("x")
来源：http://oay.hammf.cn

C#:   s.IndexOf("x")
来源：http://lqg.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pon.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://riw.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mtt.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjl.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gfp.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ihh.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wrs.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgr.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iok.chenzaomai.com

[E06] 替换子串
来源：http://poc.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lrl.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://jjb.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://maa.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://isd.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xmf.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zdh.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://shv.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://uiw.smart0.xyz

[E07] 按分隔符拆分
来源：http://bci.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fbb.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zoz.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zqc.jinghuilouyu.cn

TS:   s.split(",")
来源：http://gsp.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tfv.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://waf.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://tzj.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://okh.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://bhw.sufxvd.cn

Py:   ",".join(items)
来源：http://ldr.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://vne.sxryk.cn

JS:   items.join(",")
来源：http://xbo.sysykeji.top

TS:   items.join(",")
来源：http://pgt.hesvh.cn

Java: String.join(",", items)
来源：http://jfu.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://sjh.uphjek.com

Ruby: items.join(",")
来源：http://oed.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://lwr.cashguo.top

[E09] 去除所有空白字符
来源：http://nrv.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ddt.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eyl.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://gst.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://qti.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://goy.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lti.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://jdq.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://umf.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://odp.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cah.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hqn.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://enj.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://jkb.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://dud.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://epo.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kay.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://euv.fengsongda.top

[E11] 反转字符串
来源：http://ugx.guowangkeji.top

Py:   s[::-1]
来源：http://fct.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://whd.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://byl.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://pua.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://npp.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ywo.ehwqpu.com

Ruby: s.reverse
来源：http://isn.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ncb.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://yvm.gzhubu.top

Py:   s.count("a")
来源：http://ojq.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://pxa.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://hyz.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://xvo.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ewl.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://ipg.tianlin.xyz

Ruby: s.count("a")
来源：http://wss.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://leg.sufxvd.cn

[E13] 逐字符遍历
来源：http://qaa.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://wzg.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mif.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://nmj.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dvr.zhengqikj.top


<!-- 参考信息 -->