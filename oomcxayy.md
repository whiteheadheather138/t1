代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fdq.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://knd.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zkl.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fdt.52xcode.cn

[D11] 反转数组
来源：http://yaw.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://gun.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://mwe.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sjs.gotoacloud.top

TS:   [...arr].reverse();
来源：http://diz.xinyue.icu

Java: Collections.reverse(list);
来源：http://bun.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://gvg.daxiang520.top

Ruby: arr.reverse
来源：http://nfe.ehwqpu.com

C#:   list.Reverse();
来源：http://tou.sxryk.cn

[D12] 查找元素下标
来源：http://qaq.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://wco.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xse.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fsl.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tfs.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blx.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://vnd.tanke756.top

Ruby: arr.index(x)
来源：http://psm.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://fme.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://ihh.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zct.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fsc.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://sey.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://uoq.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tlj.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://klk.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://bed.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mba.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://ydo.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://omx.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hxi.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://sqh.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://yng.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://weh.xinyue.icu

Go:   // 手写循环
来源：http://eyz.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hqn.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gdc.zhaomingkeji.xyz

[D15] 去重
来源：http://ozu.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://efv.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://ipi.guannengcc.top

JS:   [...new Set(arr)]
来源：http://cqt.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://ieb.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rcc.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://zto.svipenyu.cn

Ruby: arr.uniq
来源：http://vqm.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://rln.316326.xyz

[D16] 求和与平均值
来源：http://hit.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayz.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vsj.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryv.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pbv.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yya.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://nna.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gsv.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://hwm.havefunace.top

[D17] 最大值与最小值
来源：http://mwr.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://uiu.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://him.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fkg.haohaochexian.top

TS:   Math.max(...arr);
来源：http://ota.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oiv.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rff.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://pra.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://dmw.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://eyw.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nwp.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://axb.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aaa.ehwqpu.com

TS:   nested.flat();
来源：http://zql.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jsb.ppjwa.cn

Go:   // 手写双层循环
来源：http://rxa.yueranfly.top

Ruby: nested.flatten
来源：http://cdq.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jvz.meibo888.top

[D19] 按字段分组
来源：http://uoh.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ntp.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxo.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kin.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kof.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uhv.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://rvc.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hmp.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tcg.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://owj.c1oappe.top

Py:   Counter(arr)
来源：http://mvx.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://ekc.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyx.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hvv.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hrh.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://cyf.nwbrower.top

Ruby: arr.tally
来源：http://zjv.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rcb.shuidangran.top

[D21] 判断是否包含某元素
来源：http://jik.hysaishi.cn

Py:   x in arr
来源：http://xku.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://mbs.vqdsnc.cn

JS:   arr.includes(x)
来源：http://fyv.dianchejie.cn

TS:   arr.includes(x)
来源：http://vrz.ybcxt.top

Java: list.contains(x)
来源：http://qty.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://egk.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://bus.hnqzz.top

C#:   list.Contains(x)
来源：http://mvg.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://bir.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eph.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ywl.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gqz.sweek.top

TS:   [...arr];
来源：http://tqk.aizwys.cn

Java: new ArrayList<>(list);
来源：http://nwm.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://dtr.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://hup.52xcode.cn

C#:   new List<int>(list);
来源：http://upm.sxryk.cn

[D23] reduce 累积计算
来源：http://bhj.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pdn.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yya.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rvd.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpz.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mid.cqqwz.cn

Go:   // 手写循环
来源：http://aox.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sps.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://odc.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://frt.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vpw.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cwk.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qap.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfc.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://npj.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://akz.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bpl.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vyv.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://wja.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eoo.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hye.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://clg.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ewy.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ibp.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyr.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jjp.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oue.feifeiyinyue.top

[D26] 数组转字符串
来源：http://fpz.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://qqd.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://yrs.cucudq.cn

JS:   arr.join(", ")
来源：http://uss.birdmap.top

TS:   arr.join(", ")
来源：http://ldo.guowangkeji.top

Java: String.join(", ", list)
来源：http://dew.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://yya.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://apv.nwbrower.top

C#:   string.Join(", ", list)
来源：http://vvz.cheryme.top

================================================================================
来源：http://zvx.xinyue.icu

E. 字符串处理
来源：http://zxq.epnwcf.com

================================================================================
来源：http://opo.dashuyun.cn

[E01] 拼接字符串
来源：http://zui.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ukk.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqn.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://els.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnm.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oah.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hiq.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qcs.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://adl.zdbjq.cn

[E02] 重复字符串
来源：http://cwa.yfazqb.com

Py:   "ab" * 3
来源：http://quz.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://djm.yuxming.cn

JS:   "ab".repeat(3)
来源：http://ncp.yonumen.top

TS:   "ab".repeat(3)
来源：http://ktg.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://ozs.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://uzf.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://yiz.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jpl.0kj1m.cn

[E03] 截取子串
来源：http://fby.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eup.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ivz.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rnp.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://mac.chenlongwang.top

Java: s.substring(1, 4)
来源：http://tzi.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qij.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://iqz.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://dif.wangshuangyany.cn

[E04] 查找子串位置
来源：http://fdf.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://tbo.yvedp.cn

PHP:  strpos($s, "x");
来源：http://ldh.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzy.iojbl.cn

TS:   s.indexOf("x")
来源：http://uye.xuanzx.com

Java: s.indexOf("x")
来源：http://aby.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://izz.cucudq.cn

Ruby: s.index("x")
来源：http://vqy.daxiang520.top

C#:   s.IndexOf("x")
来源：http://ero.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cpx.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dmd.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvd.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtz.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://imx.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oet.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xdg.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqo.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://urr.tian-w.cn

[E06] 替换子串
来源：http://xvc.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ywu.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://ptl.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fex.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://rho.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swp.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wez.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hxy.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://cxp.nanxinkj.top

[E07] 按分隔符拆分
来源：http://itp.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tgw.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://btp.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://omo.nanxinkj.top

TS:   s.split(",")
来源：http://hne.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bxa.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hfq.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://eet.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uvp.nwbrower.top

[E08] 数组按分隔符合并
来源：http://xql.guannengcc.top

Py:   ",".join(items)
来源：http://wtp.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://wtj.wangshuangyany.cn

JS:   items.join(",")
来源：http://xzi.xinyue.icu

TS:   items.join(",")
来源：http://rtc.yonumen.top

Java: String.join(",", items)
来源：http://hgm.sweek.top

Go:   strings.Join(items, ",")
来源：http://buc.jqgfzy.top

Ruby: items.join(",")
来源：http://jwi.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://pqd.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://hci.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bzr.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cyz.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ept.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://eqj.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://whk.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zut.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://pni.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ndf.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ehx.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wnr.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ybu.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://ihl.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://fkg.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://ixl.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fhv.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtz.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pci.pengpengdd.cyou

[E11] 反转字符串
来源：http://iel.quarkkingdee.top

Py:   s[::-1]
来源：http://vnt.zdqjudy.top

PHP:  strrev($s);
来源：http://gwr.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://yji.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://yiz.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vqr.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uki.redwolf501.top

Ruby: s.reverse
来源：http://wie.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://rdx.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://rci.fzhhl.top

Py:   s.count("a")
来源：http://iam.ivvv.top

PHP:  substr_count($s, "a");
来源：http://ktp.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://byz.cashguo.top

TS:   s.split("a").length - 1
来源：http://adl.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lts.tanke756.top

Go:   strings.Count(s, "a")
来源：http://few.sufxvd.cn

Ruby: s.count("a")
来源：http://unq.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://mbo.jyoumei.cn

[E13] 逐字符遍历
来源：http://tsy.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://ntm.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fyv.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pjg.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kih.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://crg.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zmq.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://raw.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oyj.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://xvd.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvv.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rnn.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wor.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rpz.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edm.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gmg.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wnk.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://exs.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://nos.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xzc.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cxl.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hus.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://quu.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cxh.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://opx.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fid.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sjc.xuetiantiany.cn

[E16] 数字千分位
来源：http://plf.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://fgt.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://bur.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://elh.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nbr.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tna.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nma.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfy.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://aty.hysaishi.cn

[E17] 首字母大写
来源：http://pnc.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ytq.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://esi.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnd.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://acw.dianchejie.cn


<!-- 参考信息 -->