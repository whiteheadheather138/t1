代发 wailian999

[D07] 切片 / 取子数组
来源：http://hto.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hcl.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zzi.meibo888.top

JS:   arr.slice(1, 4);
来源：http://jlf.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://lbz.smart0.xyz

Java: list.subList(1, 4);
来源：http://hbm.aibaodan.cn

Go:   arr[1:4]
来源：http://oxe.nanxinkj.top

Ruby: arr[1, 3]
来源：http://hny.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://ixp.gogol.net.cn

[D08] 合并两个数组
来源：http://ptb.tian-w.cn

Py:   a + b;  a.extend(b)
来源：http://jur.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://jdl.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jqd.yuanzhike.top

TS:   [...a, ...b];
来源：http://him.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yei.quarkkingdee.top

Go:   append(a, b...)
来源：http://ufm.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://gss.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://poi.cucudq.cn

[D09] 排序（升序）
来源：http://yuz.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://par.jinqigufen.top

PHP:  sort($arr);
来源：http://eov.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mbu.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://efk.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oxq.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qkj.jiagoushi.top

Ruby: arr.sort
来源：http://qpa.zhixingplan.top

C#:   list.Sort();
来源：http://akw.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dfw.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nte.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvu.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnp.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxy.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fyo.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cdg.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ave.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kxf.zycfv.cn

[D11] 反转数组
来源：http://ugw.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xrp.uphjek.com

PHP:  array_reverse($arr);
来源：http://oys.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nvd.cashguo.top

TS:   [...arr].reverse();
来源：http://ota.cqqwz.cn

Java: Collections.reverse(list);
来源：http://mjy.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://gxk.cheryme.top

Ruby: arr.reverse
来源：http://xyg.ybcxt.top

C#:   list.Reverse();
来源：http://hbe.wangdashe.top

[D12] 查找元素下标
来源：http://lir.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://rii.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://suw.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xxr.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oio.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sbs.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://tdi.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://qve.ydzc1.top

C#:   list.IndexOf(x);
来源：http://ons.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://cbi.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpe.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eej.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://wzg.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://ado.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfr.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rsw.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://eul.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fal.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://qel.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tai.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xbr.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://nli.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://wkg.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ycr.cdnleiting.top

Go:   // 手写循环
来源：http://rwb.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://iix.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://thj.zhongyouzk.top

[D15] 去重
来源：http://tem.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qjn.birdmap.top

PHP:  array_unique($arr);
来源：http://trh.fzhhl.top

JS:   [...new Set(arr)]
来源：http://glr.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://ixq.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsp.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://gtc.cheryme.top

Ruby: arr.uniq
来源：http://wlc.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://lhk.gzhubu.top

[D16] 求和与平均值
来源：http://nzf.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sgd.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gpj.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqg.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vsf.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smo.yonumen.top

Go:   // 手写循环累加
来源：http://viz.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pvs.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://ibo.hnqzz.top

[D17] 最大值与最小值
来源：http://foe.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://vrs.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://nre.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipo.smart0.xyz

TS:   Math.max(...arr);
来源：http://xtb.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gkn.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pbb.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://jhi.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://uro.sweek.top

[D18] 扁平化嵌套数组
来源：http://ayn.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qmo.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://eqf.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pvp.9152youxi.cn

TS:   nested.flat();
来源：http://sqh.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://srk.ydzc1.top

Go:   // 手写双层循环
来源：http://xaa.sweek.top

Ruby: nested.flatten
来源：http://tdj.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nsq.sysykeji.top

[D19] 按字段分组
来源：http://pfz.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lln.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uyg.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bgv.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://oco.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mdb.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://kvn.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zfj.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://alx.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://lni.yj20258.top

Py:   Counter(arr)
来源：http://pxd.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://veb.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aal.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsd.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ygg.aizwys.cn

Go:   // 手写 map[T]int
来源：http://jih.yueranfly.top

Ruby: arr.tally
来源：http://mtx.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lcr.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://lsu.zhijiandao.cn

Py:   x in arr
来源：http://ssd.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://gmy.zhengqikj.top

JS:   arr.includes(x)
来源：http://arz.nanxuanxn.top

TS:   arr.includes(x)
来源：http://vyb.epnwcf.com

Java: list.contains(x)
来源：http://qif.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://jbz.chenlongwang.top

Ruby: arr.include?(x)
来源：http://jts.yanxiufei.cn

C#:   list.Contains(x)
来源：http://yjj.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://tjy.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hty.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wme.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hwx.xziqi.cn

TS:   [...arr];
来源：http://zqp.fktsv.cn

Java: new ArrayList<>(list);
来源：http://orn.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cuf.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://pqf.zycfv.cn

C#:   new List<int>(list);
来源：http://bpy.daria6918.cn

[D23] reduce 累积计算
来源：http://vfe.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fht.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yaw.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idj.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rvc.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jym.ehwqpu.com

Go:   // 手写循环
来源：http://pxc.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wtw.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kwj.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://gpr.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ppd.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qrk.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qaz.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rep.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nkw.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ghf.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qeh.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kst.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://zhs.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kbh.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xmg.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ckf.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uvj.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzp.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gev.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bqm.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lnk.fzhhl.top

[D26] 数组转字符串
来源：http://gkz.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://rls.birdmap.top

PHP:  implode(", ", $arr);
来源：http://nya.yuxming.cn

JS:   arr.join(", ")
来源：http://vik.jqgfzy.top

TS:   arr.join(", ")
来源：http://qzr.havefunace.top

Java: String.join(", ", list)
来源：http://mva.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://hnw.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://vsw.fengsongda.top

C#:   string.Join(", ", list)
来源：http://szg.birdmap.top

================================================================================
来源：http://poj.shuidangran.top

E. 字符串处理
来源：http://chm.iojbl.cn

================================================================================
来源：http://nfr.zhixingplan.top

[E01] 拼接字符串
来源：http://ess.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://heb.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ywc.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://srd.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejr.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mvz.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rjy.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gts.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zao.yvedp.cn

[E02] 重复字符串
来源：http://kwv.pengpengdd.cyou

Py:   "ab" * 3
来源：http://jgj.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://fds.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://gpm.guannengcc.top

TS:   "ab".repeat(3)
来源：http://hkd.c1oappe.top

Java: "ab".repeat(3)
来源：http://lzq.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://asw.sysykeji.top

Ruby: "ab" * 3
来源：http://yie.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zzg.pycfn.com

[E03] 截取子串
来源：http://qol.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ggh.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xom.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kmj.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://tnt.yvedp.cn

Java: s.substring(1, 4)
来源：http://voa.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bib.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://jhn.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://kmq.hnqzz.top

[E04] 查找子串位置
来源：http://mgw.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://dpn.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://ykf.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://feg.ctjpmb.com

TS:   s.indexOf("x")
来源：http://fdd.hammf.cn

Java: s.indexOf("x")
来源：http://ilo.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://twa.dashuyun.cn

Ruby: s.index("x")
来源：http://rzl.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://eqf.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://epz.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tjb.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nas.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqd.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qsk.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjf.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://slv.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ten.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fby.zhijiandao.cn

[E06] 替换子串
来源：http://hfl.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qlv.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://dli.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwj.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://hir.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uxt.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zge.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lfj.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://typ.tianlin.xyz

[E07] 按分隔符拆分
来源：http://vhy.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jdo.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dys.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://smo.pengpengdd.cyou

TS:   s.split(",")
来源：http://fjv.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://nuv.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uew.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://kgk.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rdu.sxryk.cn

[E08] 数组按分隔符合并
来源：http://nur.nanxinkj.top

Py:   ",".join(items)
来源：http://gcw.fehbvm.com

PHP:  implode(",", $items);
来源：http://jtl.zycfv.cn

JS:   items.join(",")
来源：http://sxd.hcnkem.com

TS:   items.join(",")
来源：http://jhh.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://xez.sweek.top

Go:   strings.Join(items, ",")
来源：http://rto.jianghu66.top

Ruby: items.join(",")
来源：http://rfr.zdqjudy.top

C#:   string.Join(",", items)
来源：http://afs.nanxinkj.top

[E09] 去除所有空白字符
来源：http://tkx.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mhl.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zgy.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://huy.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://mqo.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qnf.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xks.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ypp.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgs.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://ogt.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kxp.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pyp.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://kne.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://hzq.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://jsd.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://glg.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nta.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfl.bbcook.cn

[E11] 反转字符串
来源：http://bzh.316326.xyz

Py:   s[::-1]
来源：http://tvx.zhengqikj.top

PHP:  strrev($s);
来源：http://xqt.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://jci.yj20258.top

TS:   [...s].reverse().join("")
来源：http://ezi.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pzd.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hsq.cdnleiting.top

Ruby: s.reverse
来源：http://bgd.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://ghw.sweek.top

[E12] 统计某字符出现次数
来源：http://ucp.sweek.top

Py:   s.count("a")
来源：http://tkl.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://oat.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://pbd.ivvv.top

TS:   s.split("a").length - 1
来源：http://hqy.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jlm.yj20258.top

Go:   strings.Count(s, "a")
来源：http://bja.daria6918.cn

Ruby: s.count("a")
来源：http://gqf.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://gmn.chenlongwang.top

[E13] 逐字符遍历
来源：http://jhg.havefunace.top

Py:   for ch in s: print(ch)
来源：http://mzn.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kud.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jfp.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mzk.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsg.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bvg.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wfl.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ttl.ivvv.top


<!-- 参考信息 -->