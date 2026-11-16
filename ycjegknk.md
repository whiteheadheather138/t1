代发 wailian999

[D07] 切片 / 取子数组
来源：http://bej.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ykg.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fyw.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://brn.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://vzd.mhx1999.top

Java: list.subList(1, 4);
来源：http://gdm.cashguo.top

Go:   arr[1:4]
来源：http://jmk.ydzc1.top

Ruby: arr[1, 3]
来源：http://hnv.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://ohd.hfpthk.cn

[D08] 合并两个数组
来源：http://wcw.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://ymi.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://tex.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://fbh.nanxuanxn.top

TS:   [...a, ...b];
来源：http://whr.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lzj.c1oappe.top

Go:   append(a, b...)
来源：http://zay.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://emu.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://yaz.hfpthk.cn

[D09] 排序（升序）
来源：http://vtp.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://pni.nanxuanxn.top

PHP:  sort($arr);
来源：http://omv.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kwu.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ssf.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://emm.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oeu.sweek.top

Ruby: arr.sort
来源：http://tkq.c1oappe.top

C#:   list.Sort();
来源：http://icf.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zzx.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hzs.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tjy.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkf.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oaf.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://caz.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hcu.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zmg.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mhv.tian-w.cn

[D11] 反转数组
来源：http://rjk.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ciy.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://iky.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hpl.zhijiandao.cn

TS:   [...arr].reverse();
来源：http://svb.fzhhl.top

Java: Collections.reverse(list);
来源：http://slz.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://clm.c1oappe.top

Ruby: arr.reverse
来源：http://mlt.hfpthk.cn

C#:   list.Reverse();
来源：http://fzm.cdnleiting.top

[D12] 查找元素下标
来源：http://mcn.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://mnl.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yix.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cgq.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayb.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ukx.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://hxh.yongpay.top

Ruby: arr.index(x)
来源：http://wap.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://ugn.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://kda.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nzh.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://swx.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://jrg.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://lcl.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xxk.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://umd.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://twr.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://auo.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://pfa.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://teq.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eso.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://oal.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://sdq.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ieh.hesvh.cn

Go:   // 手写循环
来源：http://wcr.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://vxo.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://myt.yonumen.top

[D15] 去重
来源：http://bej.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yyq.jyoumei.cn

PHP:  array_unique($arr);
来源：http://raf.fktsv.cn

JS:   [...new Set(arr)]
来源：http://zgk.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://ndy.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jtx.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://bca.sxryk.cn

Ruby: arr.uniq
来源：http://ptb.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://wpy.yuxming.cn

[D16] 求和与平均值
来源：http://uof.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ouh.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lac.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifg.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tnk.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://trv.jianghu66.top

Go:   // 手写循环累加
来源：http://bbr.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ocq.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://hfu.hnqzz.top

[D17] 最大值与最小值
来源：http://woz.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://xsx.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://qjc.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vkg.cheryme.top

TS:   Math.max(...arr);
来源：http://dck.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lsi.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ple.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://fnd.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://cas.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://bsc.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xud.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://zqj.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qoq.daria6918.cn

TS:   nested.flat();
来源：http://oio.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fqa.yangfankeji.com

Go:   // 手写双层循环
来源：http://kwv.svipenyu.cn

Ruby: nested.flatten
来源：http://ugu.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xsl.zdqjudy.top

[D19] 按字段分组
来源：http://bmk.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mmf.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fjv.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lkz.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uqs.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tat.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://czr.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://bsv.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vjs.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://zpm.yongpay.top

Py:   Counter(arr)
来源：http://kxj.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://drd.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyb.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gby.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://edx.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://uwd.uphjek.com

Ruby: arr.tally
来源：http://qgp.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dxb.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://ejm.c1oappe.top

Py:   x in arr
来源：http://qon.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://dhu.zycfv.cn

JS:   arr.includes(x)
来源：http://pwv.chenlongwang.top

TS:   arr.includes(x)
来源：http://hwx.ydzc1.top

Java: list.contains(x)
来源：http://nxv.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://gif.birdmap.top

Ruby: arr.include?(x)
来源：http://yru.yuanzhike.top

C#:   list.Contains(x)
来源：http://qdx.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://txu.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mtd.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mna.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wnm.0kj1m.cn

TS:   [...arr];
来源：http://jkz.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://lmr.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://nuk.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://tow.dianchejie.cn

C#:   new List<int>(list);
来源：http://hus.yueranfly.top

[D23] reduce 累积计算
来源：http://izk.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dvb.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pdi.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gil.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://isk.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://wke.yvedp.cn

Go:   // 手写循环
来源：http://jwv.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://omm.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nhp.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://fxx.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rqj.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ott.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myn.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dyd.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rdl.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bzj.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://euu.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hpf.yongpay.top

[D25] Set 集合去重与交并差
来源：http://nef.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mhp.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nmp.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oxn.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ndk.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vru.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bqi.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bdp.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://upl.guowangkeji.top

[D26] 数组转字符串
来源：http://xac.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://siw.yj20258.top

PHP:  implode(", ", $arr);
来源：http://toz.jianghu66.top

JS:   arr.join(", ")
来源：http://uic.jinqigufen.top

TS:   arr.join(", ")
来源：http://fcw.zdbjq.cn

Java: String.join(", ", list)
来源：http://nrl.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://gpm.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://zfe.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://ejf.shanyushiyangtech.top

================================================================================
来源：http://jnf.zdqjudy.top

E. 字符串处理
来源：http://mrx.wangshuangyany.cn

================================================================================
来源：http://mcv.svipenyu.cn

[E01] 拼接字符串
来源：http://bwv.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lse.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nnl.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lkm.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://epb.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qpe.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rcm.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gci.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://swi.zhongyouzk.top

[E02] 重复字符串
来源：http://vrk.tian-w.cn

Py:   "ab" * 3
来源：http://lqf.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://shc.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://dlj.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://yeb.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://dfm.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://azy.fzhhl.top

Ruby: "ab" * 3
来源：http://phr.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gsp.svipenyu.cn

[E03] 截取子串
来源：http://zwb.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uau.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mdt.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://isi.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://ajx.aizwys.cn

Java: s.substring(1, 4)
来源：http://doa.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lvb.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zja.tarul.cn

C#:   s.Substring(1, 3)
来源：http://gxo.iojbl.cn

[E04] 查找子串位置
来源：http://lij.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://tua.meibo888.top

PHP:  strpos($s, "x");
来源：http://hjc.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oxo.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://drl.xinyue.icu

Java: s.indexOf("x")
来源：http://uka.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://cnu.fzhhl.top

Ruby: s.index("x")
来源：http://pxv.c1oappe.top

C#:   s.IndexOf("x")
来源：http://pqq.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ehm.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rqc.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hrm.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bri.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nhe.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iha.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hqe.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zqy.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zkh.smart0.xyz

[E06] 替换子串
来源：http://hqq.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wew.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://cay.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://owj.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://sbr.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npy.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qqt.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://efc.tarul.cn

C#:   s.Replace("a", "b")
来源：http://crc.yuxming.cn

[E07] 按分隔符拆分
来源：http://ptr.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ykk.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bwj.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lti.jqgfzy.top

TS:   s.split(",")
来源：http://ycm.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://zey.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wni.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://neo.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gll.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://odv.guowangkeji.top

Py:   ",".join(items)
来源：http://vvs.zdqjudy.top

PHP:  implode(",", $items);
来源：http://mcy.tianlin.xyz

JS:   items.join(",")
来源：http://wfw.zhijiandao.cn

TS:   items.join(",")
来源：http://ewq.snrcjt.cn

Java: String.join(",", items)
来源：http://wto.meibo888.top

Go:   strings.Join(items, ",")
来源：http://oeb.dashuyun.cn

Ruby: items.join(",")
来源：http://hjz.hcnkem.com

C#:   string.Join(",", items)
来源：http://yka.vehdjk.com

[E09] 去除所有空白字符
来源：http://vqv.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://izg.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rls.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://nvf.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://kvf.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ops.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ojt.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://biw.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vtj.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://kbu.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://twm.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qrt.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://wcc.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://lwz.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://jxx.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bnv.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qdn.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nkh.fktsv.cn

[E11] 反转字符串
来源：http://per.snrcjt.cn

Py:   s[::-1]
来源：http://rtf.hfpthk.cn

PHP:  strrev($s);
来源：http://htx.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://tpj.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://ulh.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xgl.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kay.zhixingplan.top

Ruby: s.reverse
来源：http://jwl.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://ooy.yonumen.top

[E12] 统计某字符出现次数
来源：http://lir.yj202588.top

Py:   s.count("a")
来源：http://otv.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://wyo.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://ygh.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://drm.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fex.birdmap.top

Go:   strings.Count(s, "a")
来源：http://mjh.aibaodan.cn

Ruby: s.count("a")
来源：http://qjn.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://uyw.yvedp.cn

[E13] 逐字符遍历
来源：http://coq.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://vnv.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vlr.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hxk.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dyh.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xiy.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jjn.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kxk.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gpv.shuidangran.top


<!-- 参考信息 -->