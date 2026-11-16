代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vns.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ogi.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pmw.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iak.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ggr.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pjd.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://evb.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sxb.yj20258.top

[D11] 反转数组
来源：http://ebg.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://jbx.hesvh.cn

PHP:  array_reverse($arr);
来源：http://rtz.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zuc.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://omw.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://nuz.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://vrf.zhengqikj.top

Ruby: arr.reverse
来源：http://tlh.jianghu66.top

C#:   list.Reverse();
来源：http://ard.zhixingplan.top

[D12] 查找元素下标
来源：http://cfe.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://cjq.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lzm.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://juc.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sih.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uwy.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://bvc.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://adn.sxryk.cn

C#:   list.IndexOf(x);
来源：http://efj.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://svv.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xeq.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qwk.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://hhb.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://qnq.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dto.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mtp.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://ujx.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jtu.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://baq.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xqw.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hky.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ewj.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://gvx.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ayp.chenlongwang.top

Go:   // 手写循环
来源：http://zja.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fnn.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zwd.jlsjyb.cn

[D15] 去重
来源：http://pqp.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ljj.yj20258.top

PHP:  array_unique($arr);
来源：http://api.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://bbr.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://jfc.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hzs.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vwr.yonumen.top

Ruby: arr.uniq
来源：http://gmu.yj202588.top

C#:   list.Distinct().ToList()
来源：http://cgw.jinqigfzy.top

[D16] 求和与平均值
来源：http://pzs.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pro.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oso.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://brb.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fdm.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kya.bbcook.cn

Go:   // 手写循环累加
来源：http://mkf.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mfy.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://kps.zhengqikj.top

[D17] 最大值与最小值
来源：http://ahs.yongpay.top

Py:   max(arr);  min(arr)
来源：http://mtq.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://wtk.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bhn.havefunace.top

TS:   Math.max(...arr);
来源：http://swd.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ejv.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vjh.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://zde.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://meo.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://zsu.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hty.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://dws.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yda.jianghu66.top

TS:   nested.flat();
来源：http://ofz.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvn.sxryk.cn

Go:   // 手写双层循环
来源：http://yym.daria6918.cn

Ruby: nested.flatten
来源：http://qgp.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qsj.guowangkeji.top

[D19] 按字段分组
来源：http://vvn.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fui.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ndy.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xuv.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gcs.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eea.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://mcj.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zpo.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uts.havefunace.top

[D20] 统计每个元素出现次数
来源：http://wys.sufxvd.cn

Py:   Counter(arr)
来源：http://xeg.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://pjr.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zdi.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xec.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gyj.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://mzr.sufxvd.cn

Ruby: arr.tally
来源：http://gag.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fgq.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://gsx.fengsongda.top

Py:   x in arr
来源：http://irc.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://wrt.cheryme.top

JS:   arr.includes(x)
来源：http://ked.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://azy.sweek.top

Java: list.contains(x)
来源：http://cwx.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://cxy.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://eif.0kj1m.cn

C#:   list.Contains(x)
来源：http://kwm.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://ybf.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kbu.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jmg.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gen.aibaodan.cn

TS:   [...arr];
来源：http://yyr.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://fwi.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://isy.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://ocl.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://btb.yueranfly.top

[D23] reduce 累积计算
来源：http://wba.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yjy.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ixh.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pvf.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msk.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sfm.chenzaomai.com

Go:   // 手写循环
来源：http://lxv.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jpr.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fpy.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://ilx.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dui.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://agr.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iaw.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rpj.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sgk.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bxd.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hod.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qka.sweek.top

[D25] Set 集合去重与交并差
来源：http://tdr.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ezl.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mxb.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hjc.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ifp.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://diu.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qeh.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ren.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://udr.yueranfly.top

[D26] 数组转字符串
来源：http://uki.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://rym.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://vlt.jiagoushi.top

JS:   arr.join(", ")
来源：http://pmn.sjlbkw.cn

TS:   arr.join(", ")
来源：http://wkf.yj202588.top

Java: String.join(", ", list)
来源：http://snm.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://hyf.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://atr.redwolf501.top

C#:   string.Join(", ", list)
来源：http://dlv.zhixingplan.top

================================================================================
来源：http://uhc.zhengqikj.top

E. 字符串处理
来源：http://drp.ywan-chungtsiang.top

================================================================================
来源：http://ggb.ydjk.org.cn

[E01] 拼接字符串
来源：http://klb.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qmh.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nbx.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ckf.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://saq.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sva.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ppd.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ynh.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fuw.yj202588.top

[E02] 重复字符串
来源：http://qux.zdqjudy.top

Py:   "ab" * 3
来源：http://amg.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://nlv.fktsv.cn

JS:   "ab".repeat(3)
来源：http://xhz.meibo888.top

TS:   "ab".repeat(3)
来源：http://wvx.chenlongwang.top

Java: "ab".repeat(3)
来源：http://uce.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://ine.gogol.net.cn

Ruby: "ab" * 3
来源：http://tei.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qfj.zhaomingkeji.xyz

[E03] 截取子串
来源：http://pwl.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://udp.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lpw.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tum.316326.xyz

TS:   s.slice(1, 4)
来源：http://ugw.aibaodan.cn

Java: s.substring(1, 4)
来源：http://ere.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xws.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://xac.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://vlq.ydzc1.top

[E04] 查找子串位置
来源：http://bqh.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://ocf.fktsv.cn

PHP:  strpos($s, "x");
来源：http://tve.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rar.cdnleiting.top

TS:   s.indexOf("x")
来源：http://kdr.snrcjt.cn

Java: s.indexOf("x")
来源：http://uvg.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://hjd.zhixingplan.top

Ruby: s.index("x")
来源：http://kqq.ybcxt.top

C#:   s.IndexOf("x")
来源：http://mtv.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oct.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://agc.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fgp.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://omr.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kyr.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jur.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezh.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lac.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ngl.zhaomingkeji.xyz

[E06] 替换子串
来源：http://mso.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mta.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://wlp.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wte.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://vvp.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swg.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rgd.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lxd.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://ycn.mhx1999.top

[E07] 按分隔符拆分
来源：http://ryc.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://inf.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rrv.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lld.ydzc1.top

TS:   s.split(",")
来源：http://mgl.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kgk.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ggj.tarul.cn

Ruby: s.split(",");  s.split
来源：http://rsl.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ets.daria6918.cn

[E08] 数组按分隔符合并
来源：http://gpk.gotoacloud.top

Py:   ",".join(items)
来源：http://siv.gzhubu.top

PHP:  implode(",", $items);
来源：http://usi.vehdjk.com

JS:   items.join(",")
来源：http://juk.jianghu66.top

TS:   items.join(",")
来源：http://xct.jinqigfzy.top

Java: String.join(",", items)
来源：http://aca.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://ejf.chenlongwang.top

Ruby: items.join(",")
来源：http://kiv.0kj1m.cn

C#:   string.Join(",", items)
来源：http://gpi.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://ppm.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ncy.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zss.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://cok.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://olw.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://ywc.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tho.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://qzf.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vdn.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://fuq.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rkz.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pix.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://tac.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://zut.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://mjr.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://etz.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ozr.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uty.chenlongwang.top

[E11] 反转字符串
来源：http://voh.nanxuanxn.top

Py:   s[::-1]
来源：http://ktd.hnxiangtu.top

PHP:  strrev($s);
来源：http://ikw.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://huf.cashguo.top

TS:   [...s].reverse().join("")
来源：http://llo.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xrm.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ctj.sufxvd.cn

Ruby: s.reverse
来源：http://vnh.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://hxn.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://lxd.316326.xyz

Py:   s.count("a")
来源：http://gym.yonumen.top

PHP:  substr_count($s, "a");
来源：http://dsh.shuidangran.top

JS:   s.split("a").length - 1
来源：http://obn.birdmap.top

TS:   s.split("a").length - 1
来源：http://vpy.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jgv.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://jrz.ehwqpu.com

Ruby: s.count("a")
来源：http://sqf.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://yqw.iojbl.cn

[E13] 逐字符遍历
来源：http://xrh.tanke756.top

Py:   for ch in s: print(ch)
来源：http://rki.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://odn.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://tqj.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://see.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ayj.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jas.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oyj.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lwx.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://qbj.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rbc.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ufb.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ipd.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kpf.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tzl.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yyn.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zja.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ltx.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://fqi.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dbm.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ppp.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://drs.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://zah.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dpi.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fqb.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fya.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zpv.shanyushiyangtech.top

[E16] 数字千分位
来源：http://npj.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://puk.svipenyu.cn

PHP:  number_format(1234567);
来源：http://mzp.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vxj.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qhh.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mku.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fqc.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vxx.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://noh.sweek.top

[E17] 首字母大写
来源：http://qur.zhoulong.xyz


<!-- 参考信息 -->