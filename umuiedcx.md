代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xwr.redwolf501.top

Ruby: arr.sort
来源：http://ocl.redwolf501.top

C#:   list.Sort();
来源：http://dot.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lmb.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://axr.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yai.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rdz.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nwh.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ffa.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jlw.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pda.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uzc.zhijiandao.cn

[D11] 反转数组
来源：http://ual.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://dgg.uphjek.com

PHP:  array_reverse($arr);
来源：http://gvk.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zge.ppjwa.cn

TS:   [...arr].reverse();
来源：http://kjw.tarul.cn

Java: Collections.reverse(list);
来源：http://ded.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://mbn.andypj.xyz

Ruby: arr.reverse
来源：http://gta.gotoacloud.top

C#:   list.Reverse();
来源：http://wav.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://twl.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://gli.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tka.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twp.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dam.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vsj.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://bjz.epnwcf.com

Ruby: arr.index(x)
来源：http://utn.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://dgj.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://rso.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://clw.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbn.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://azv.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://vcj.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ggm.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hyv.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://bpa.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bws.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://flm.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tsq.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://veh.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://sxk.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://oem.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dzl.ydjk.org.cn

Go:   // 手写循环
来源：http://eqn.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://wac.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tbm.zdqjudy.top

[D15] 去重
来源：http://kpj.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://buf.316326.xyz

PHP:  array_unique($arr);
来源：http://mlk.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://ilf.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://pqz.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ooh.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cag.snrcjt.cn

Ruby: arr.uniq
来源：http://bxm.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://lah.cashguo.top

[D16] 求和与平均值
来源：http://mws.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nbu.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cou.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ynd.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqt.tarul.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gxc.fzhhl.top

Go:   // 手写循环累加
来源：http://xuc.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pgt.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://loz.gzhubu.top

[D17] 最大值与最小值
来源：http://ice.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://bak.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://ylj.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://elq.yuxming.cn

TS:   Math.max(...arr);
来源：http://esb.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://brv.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cri.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://jey.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://cod.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://mah.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ngv.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://sol.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://htu.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://vdy.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kts.jianghu66.top

Go:   // 手写双层循环
来源：http://sqa.kuanghao11.cn

Ruby: nested.flatten
来源：http://gpg.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqn.dashuyun.cn

[D19] 按字段分组
来源：http://kow.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pfw.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zra.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lnk.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nyp.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oji.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://twg.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qti.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nod.birdmap.top

[D20] 统计每个元素出现次数
来源：http://bbv.nanxinkj.top

Py:   Counter(arr)
来源：http://phf.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://lak.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tkk.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mkm.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://raj.xziqi.cn

Go:   // 手写 map[T]int
来源：http://kpp.jyoumei.cn

Ruby: arr.tally
来源：http://ayh.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://too.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://snp.zhoulong.xyz

Py:   x in arr
来源：http://rqf.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://jth.chenzaomai.com

JS:   arr.includes(x)
来源：http://xqw.hnxiangtu.top

TS:   arr.includes(x)
来源：http://kxx.jlsjyb.cn

Java: list.contains(x)
来源：http://wyu.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://wam.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://pgy.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://buz.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://zar.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yyr.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cof.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cpo.ivvv.top

TS:   [...arr];
来源：http://qlb.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://dsa.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://rrk.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://frs.xinyue.icu

C#:   new List<int>(list);
来源：http://ykc.zhixingplan.top

[D23] reduce 累积计算
来源：http://bpw.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqp.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://voz.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uqb.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtl.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lrh.iojbl.cn

Go:   // 手写循环
来源：http://fpr.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fdp.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://icj.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://gei.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jmj.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://clk.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://glx.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pzc.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kcm.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oda.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zlx.jinqigfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wso.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://vnr.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://djs.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://quq.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hqw.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wlx.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bqw.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://asr.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uju.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://thf.jiagoushi.top

[D26] 数组转字符串
来源：http://lbl.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://vrh.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://sfz.guowangkeji.top

JS:   arr.join(", ")
来源：http://jfp.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://owc.bjfxy.top

Java: String.join(", ", list)
来源：http://kxd.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://gzb.52xcode.cn

Ruby: arr.join(", ")
来源：http://wct.vehdjk.com

C#:   string.Join(", ", list)
来源：http://kzv.smart0.xyz

================================================================================
来源：http://ifp.tianlin.xyz

E. 字符串处理
来源：http://vzd.hywenlv.cn

================================================================================
来源：http://jyh.fktsv.cn

[E01] 拼接字符串
来源：http://qoi.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gxy.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lja.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tey.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ijo.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://moi.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ynk.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jby.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ozs.zdqjudy.top

[E02] 重复字符串
来源：http://inv.sxryk.cn

Py:   "ab" * 3
来源：http://ikz.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://ytz.fehbvm.com

JS:   "ab".repeat(3)
来源：http://vow.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://xdj.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://rtp.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ihx.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://efy.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ybq.snrcjt.cn

[E03] 截取子串
来源：http://ycd.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lai.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oga.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://frb.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://pco.yonumen.top

Java: s.substring(1, 4)
来源：http://wnn.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpq.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://jsd.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://rez.hywenlv.cn

[E04] 查找子串位置
来源：http://mhi.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://see.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://kgy.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fqf.sxryk.cn

TS:   s.indexOf("x")
来源：http://eqh.316326.xyz

Java: s.indexOf("x")
来源：http://uzg.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://hqy.hywenlv.cn

Ruby: s.index("x")
来源：http://xvj.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://yfj.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlo.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qfi.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xzw.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lme.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgn.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yrh.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://llk.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wlv.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dyy.fehbvm.com

[E06] 替换子串
来源：http://riq.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qkj.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://hbp.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iav.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://rgi.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxj.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kio.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avx.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://ral.ydzc1.top

[E07] 按分隔符拆分
来源：http://tiq.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zcs.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yfq.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ann.nanxinkj.top

TS:   s.split(",")
来源：http://erq.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://vst.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nvx.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://xza.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ylk.shuidangran.top

[E08] 数组按分隔符合并
来源：http://oma.aibaodan.cn

Py:   ",".join(items)
来源：http://uuv.hnqzz.top

PHP:  implode(",", $items);
来源：http://rer.shzxlz.cn

JS:   items.join(",")
来源：http://gdo.ydjk.org.cn

TS:   items.join(",")
来源：http://mbd.gogol.net.cn

Java: String.join(",", items)
来源：http://lcb.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://niu.sweek.top

Ruby: items.join(",")
来源：http://ocg.andypj.xyz

C#:   string.Join(",", items)
来源：http://tyb.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://xet.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sml.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cpd.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://xpi.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://ieb.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://pth.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://stz.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://qxi.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vkp.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://twg.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rjj.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bjk.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://bsj.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://luz.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://rmy.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://woq.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uyo.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xip.mhx1999.top

[E11] 反转字符串
来源：http://utt.jinqigufen.top

Py:   s[::-1]
来源：http://tbb.sxryk.cn

PHP:  strrev($s);
来源：http://fme.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://bxl.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://cbd.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cho.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yiy.xinyue.icu

Ruby: s.reverse
来源：http://knb.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://ifl.ydzc1.top

[E12] 统计某字符出现次数
来源：http://nsd.316326.xyz

Py:   s.count("a")
来源：http://cgb.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://cnc.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://zxv.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://fle.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kyg.havefunace.top

Go:   strings.Count(s, "a")
来源：http://lcw.quarkkingdee.top

Ruby: s.count("a")
来源：http://xms.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://kmd.tian-w.cn

[E13] 逐字符遍历
来源：http://lei.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://fmw.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dnu.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhy.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ygz.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qef.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hmd.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eex.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lqa.ydzc1.top

[E14] URL 编码与 Base64
来源：http://svl.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pae.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://zvm.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wli.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zmz.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mej.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aik.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dtv.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://okt.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://mzc.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ezn.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kjs.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gzx.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aem.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhn.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lfy.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bbj.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kax.yuanzhike.top

[E16] 数字千分位
来源：http://msr.uphjek.com

Py:   f"{1234567:,}"
来源：http://nxi.birdmap.top

PHP:  number_format(1234567);
来源：http://xpx.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ykr.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lsd.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lhp.yj20258.top


<!-- 参考信息 -->