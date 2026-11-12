代发 wailian999

Py:   len(arr)
来源：http://ofp.sjlbkw.cn

PHP:  count($arr);
来源：http://sct.birdmap.top

JS:   arr.length
来源：http://jly.zdbjq.cn

TS:   arr.length
来源：http://mvy.cheryme.top

Java: list.size();
来源：http://spj.birdmap.top

Go:   len(arr)
来源：http://ksv.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://buj.epnwcf.com

C#:   list.Count;
来源：http://tha.hesvh.cn

[D07] 切片 / 取子数组
来源：http://lqr.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nlq.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mmb.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://iel.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://sgi.nanxinkj.top

Java: list.subList(1, 4);
来源：http://ajt.guannengcc.top

Go:   arr[1:4]
来源：http://kkf.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://uzk.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://gva.pycfn.com

[D08] 合并两个数组
来源：http://uor.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://dqd.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://ilt.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://krd.zdbjq.cn

TS:   [...a, ...b];
来源：http://dzh.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pjl.tian-w.cn

Go:   append(a, b...)
来源：http://fhx.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://ozp.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://xnp.mhx1999.top

[D09] 排序（升序）
来源：http://vbn.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://mal.hnqzz.top

PHP:  sort($arr);
来源：http://sor.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://evu.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ztn.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://yur.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bzs.gaohongyu789.top

Ruby: arr.sort
来源：http://tcn.jianghu66.top

C#:   list.Sort();
来源：http://jol.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mog.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://von.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hxb.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ths.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xor.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uyd.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sro.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mgs.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://azt.xinyue.icu

[D11] 反转数组
来源：http://bng.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://tcv.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://egq.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yus.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://smn.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://lzl.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://aaa.tianlin.xyz

Ruby: arr.reverse
来源：http://dua.0kj1m.cn

C#:   list.Reverse();
来源：http://nup.wangshuangyany.cn

[D12] 查找元素下标
来源：http://lpe.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://mxd.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://exj.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjw.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ckh.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gvc.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://uct.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://yhp.yuxming.cn

C#:   list.IndexOf(x);
来源：http://tib.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://yub.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rzi.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sbm.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://kaw.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://kwy.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://put.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yku.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://jwt.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eap.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://xaz.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kxk.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uss.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://vgj.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://ztp.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pao.hywenlv.cn

Go:   // 手写循环
来源：http://rmh.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ypr.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://emn.xuanzx.com

[D15] 去重
来源：http://vnu.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eff.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://nec.ivvv.top

JS:   [...new Set(arr)]
来源：http://wti.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://nbb.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sco.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://ilv.sufxvd.cn

Ruby: arr.uniq
来源：http://mtv.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://ovy.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://hwn.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://znu.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://clg.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://otk.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyx.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dyx.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://oki.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ven.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://ibk.cqqwz.cn

[D17] 最大值与最小值
来源：http://ghk.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://guk.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://hys.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pvy.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://mqb.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vuf.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://brr.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://pim.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://xjv.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://hzn.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kha.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://frl.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oxi.fengsongda.top

TS:   nested.flat();
来源：http://ckj.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sam.sjlbkw.cn

Go:   // 手写双层循环
来源：http://esh.ivvv.top

Ruby: nested.flatten
来源：http://crf.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kpw.chenzaomai.com

[D19] 按字段分组
来源：http://qot.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fjd.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ijz.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kop.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bxa.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yez.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://nrg.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzx.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://igv.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://kve.yj20258888.top

Py:   Counter(arr)
来源：http://rot.nwbrower.top

PHP:  array_count_values($arr);
来源：http://hzy.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bni.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyr.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uuq.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://giz.xuetiantiany.cn

Ruby: arr.tally
来源：http://rxg.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dio.pycfn.com

[D21] 判断是否包含某元素
来源：http://izn.cucudq.cn

Py:   x in arr
来源：http://evx.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://pcf.ivvv.top

JS:   arr.includes(x)
来源：http://avt.bjfxy.top

TS:   arr.includes(x)
来源：http://asv.epnwcf.com

Java: list.contains(x)
来源：http://kzi.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://gtb.andypj.xyz

Ruby: arr.include?(x)
来源：http://tmo.hnxiangtu.top

C#:   list.Contains(x)
来源：http://bgi.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://bnp.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mfi.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wil.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://buc.wangshuangyany.cn

TS:   [...arr];
来源：http://jok.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://cix.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://nmv.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ytb.fzhhl.top

C#:   new List<int>(list);
来源：http://kva.dianchejie.cn

[D23] reduce 累积计算
来源：http://wee.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rxr.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rgp.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tvo.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvg.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://gel.cdnleiting.top

Go:   // 手写循环
来源：http://lzp.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://izq.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gox.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://zas.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ipb.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qcf.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kec.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zhh.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dyx.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kfh.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://abp.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://liu.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://ufg.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kdc.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fkf.fehbvm.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://seh.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lxl.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ogp.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kyj.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jna.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qhy.guowangkeji.top

[D26] 数组转字符串
来源：http://rgu.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://yrk.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://gmx.shzxlz.cn

JS:   arr.join(", ")
来源：http://sek.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://hue.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://pcl.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://ndi.yonumen.top

Ruby: arr.join(", ")
来源：http://vjd.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://ngm.zhongyouzk.top

================================================================================
来源：http://vus.shuidangran.top

E. 字符串处理
来源：http://daw.fengsongda.top

================================================================================
来源：http://xbz.ehwqpu.com

[E01] 拼接字符串
来源：http://yvp.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jsf.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zss.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://avp.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tmg.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://goq.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eev.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://irb.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://flh.yueranfly.top

[E02] 重复字符串
来源：http://cbm.daria6918.cn

Py:   "ab" * 3
来源：http://pmc.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://ncs.cucudq.cn

JS:   "ab".repeat(3)
来源：http://hck.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://tip.shuidangran.top

Java: "ab".repeat(3)
来源：http://sto.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://oda.svipenyu.cn

Ruby: "ab" * 3
来源：http://dck.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tyb.uphjek.com

[E03] 截取子串
来源：http://kng.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mce.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://khj.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgo.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://xmt.mhx1999.top

Java: s.substring(1, 4)
来源：http://edm.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://log.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://nsn.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://dtc.yangfankeji.com

[E04] 查找子串位置
来源：http://ioi.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://cby.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://iyg.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iej.xinyue.icu

TS:   s.indexOf("x")
来源：http://pke.daria6918.cn

Java: s.indexOf("x")
来源：http://kfd.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://tip.kuanghao11.cn

Ruby: s.index("x")
来源：http://mec.yj202588.top

C#:   s.IndexOf("x")
来源：http://svj.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wwy.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://auz.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pxc.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xov.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gnc.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxg.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://plo.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fbh.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wse.shanyushiyangkeji.top

[E06] 替换子串
来源：http://jzm.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fsd.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://aqv.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izi.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://moa.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qgn.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kmf.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zax.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://bjv.guannengcc.top

[E07] 按分隔符拆分
来源：http://jgy.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aoa.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cvo.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rct.fanxiaobao.xyz

TS:   s.split(",")
来源：http://mlu.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://rek.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fky.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://uth.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fyd.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://upj.jinqigufen.top

Py:   ",".join(items)
来源：http://iys.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://jri.c1oappe.top

JS:   items.join(",")
来源：http://ona.redwolf501.top

TS:   items.join(",")
来源：http://xog.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://rqt.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://gdx.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://oqk.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://qxf.ctjpmb.com

[E09] 去除所有空白字符
来源：http://nma.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://man.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfe.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://rcq.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://rxy.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://lwz.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mcx.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://wyg.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yxu.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://ity.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://anh.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ukt.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://tnj.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://pxh.ivvv.top

Java: String.format("%03d", 7)
来源：http://pmt.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wek.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qov.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqc.pycfn.com

[E11] 反转字符串
来源：http://xco.sxryk.cn

Py:   s[::-1]
来源：http://zqm.jyoumei.cn

PHP:  strrev($s);
来源：http://tsf.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://kee.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://wmn.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bsd.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uav.zhixingplan.top

Ruby: s.reverse
来源：http://qca.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://fvp.52xcode.cn

[E12] 统计某字符出现次数
来源：http://kie.bbcook.cn

Py:   s.count("a")
来源：http://mly.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://yiz.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://rlj.yfazqb.com

TS:   s.split("a").length - 1
来源：http://sku.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://krg.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://lnc.cashguo.top

Ruby: s.count("a")
来源：http://yey.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://czb.sweek.top

[E13] 逐字符遍历
来源：http://wza.9152youxi.cn


<!-- 参考信息 -->