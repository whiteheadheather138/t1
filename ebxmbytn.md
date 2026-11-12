代发 wailian999

C#:   list.Reverse();
来源：http://nxm.zhiwuduotai.top

[D12] 查找元素下标
来源：http://gsg.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://htz.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://grn.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://czh.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymx.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sia.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://mlu.jinqigufen.top

Ruby: arr.index(x)
来源：http://pov.cucudq.cn

C#:   list.IndexOf(x);
来源：http://tuh.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://kux.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oak.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gfy.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://lth.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://cpy.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lmr.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nuc.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lfg.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cla.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://kat.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eha.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qza.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://thh.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://bkx.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ubf.tarul.cn

Go:   // 手写循环
来源：http://nzo.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://ndh.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ftw.shanyushiyangkeji.top

[D15] 去重
来源：http://joo.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vsn.yvedp.cn

PHP:  array_unique($arr);
来源：http://ntv.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://gwk.yfazqb.com

TS:   [...new Set(arr)]
来源：http://xah.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lev.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://url.redwolf501.top

Ruby: arr.uniq
来源：http://rth.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://dih.cucudq.cn

[D16] 求和与平均值
来源：http://fby.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bhe.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oua.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rtz.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujf.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rgx.yuxming.cn

Go:   // 手写循环累加
来源：http://bxw.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://deh.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://rmz.nwbrower.top

[D17] 最大值与最小值
来源：http://acc.yongpay.top

Py:   max(arr);  min(arr)
来源：http://uxp.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://ide.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zcl.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://byh.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://imr.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cog.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://fhg.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://mso.tarul.cn

[D18] 扁平化嵌套数组
来源：http://lru.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hjl.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://dbr.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fvg.nwbrower.top

TS:   nested.flat();
来源：http://ktm.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozd.meibo888.top

Go:   // 手写双层循环
来源：http://zsu.hcnkem.com

Ruby: nested.flatten
来源：http://pcc.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uwh.shangyingyoupin.top

[D19] 按字段分组
来源：http://uyi.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bxd.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yge.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuq.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mud.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lui.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://xts.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fei.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tyb.pycfn.com

[D20] 统计每个元素出现次数
来源：http://khj.fengsongda.top

Py:   Counter(arr)
来源：http://tdg.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://fcx.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bca.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvs.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ewx.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://fio.jianghu66.top

Ruby: arr.tally
来源：http://ohm.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yye.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://yep.hnxiangtu.top

Py:   x in arr
来源：http://ogd.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://glr.yj20258888.top

JS:   arr.includes(x)
来源：http://uwv.andypj.xyz

TS:   arr.includes(x)
来源：http://xso.fzhhl.top

Java: list.contains(x)
来源：http://ypp.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://yqk.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://ndh.hywenlv.cn

C#:   list.Contains(x)
来源：http://nko.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://ucv.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yse.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fwl.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://str.yanxiufei.cn

TS:   [...arr];
来源：http://ccc.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://vwt.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://nqg.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://oye.ydzc1.top

C#:   new List<int>(list);
来源：http://gla.nanxinkj.top

[D23] reduce 累积计算
来源：http://cxa.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vky.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lhq.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojn.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uro.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kxn.jlsjyb.cn

Go:   // 手写循环
来源：http://fno.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xvz.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zsa.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://xhb.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hxe.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://arl.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://izr.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cmv.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zdx.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vtv.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wpd.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ofb.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://iyy.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cph.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gia.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yoh.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gyq.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vkl.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fxa.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jwd.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kcs.yongpay.top

[D26] 数组转字符串
来源：http://car.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://rzo.yongpay.top

PHP:  implode(", ", $arr);
来源：http://qht.yfazqb.com

JS:   arr.join(", ")
来源：http://eck.jinqigufen.top

TS:   arr.join(", ")
来源：http://ltu.dianchejie.cn

Java: String.join(", ", list)
来源：http://icg.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://kwk.haohaochexian.top

Ruby: arr.join(", ")
来源：http://tdb.meibo888.top

C#:   string.Join(", ", list)
来源：http://pke.hammf.cn

================================================================================
来源：http://uzr.mhx1999.top

E. 字符串处理
来源：http://hxt.epnwcf.com

================================================================================
来源：http://wmj.cheryme.top

[E01] 拼接字符串
来源：http://wcy.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ggz.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xgv.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://snj.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://elr.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hno.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tip.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gmy.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fbf.fzhhl.top

[E02] 重复字符串
来源：http://anf.shuidangran.top

Py:   "ab" * 3
来源：http://kyc.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://jdi.yvedp.cn

JS:   "ab".repeat(3)
来源：http://nzf.tian-w.cn

TS:   "ab".repeat(3)
来源：http://mrg.yfazqb.com

Java: "ab".repeat(3)
来源：http://yjc.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ayb.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://kbz.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cxs.fanxiaobao.xyz

[E03] 截取子串
来源：http://ber.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mgo.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qlo.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zik.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://noy.cashguo.top

Java: s.substring(1, 4)
来源：http://vmp.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tbv.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://grn.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://fna.tanke756.top

[E04] 查找子串位置
来源：http://ehj.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://vff.yj20258.top

PHP:  strpos($s, "x");
来源：http://xrr.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xzi.aibaodan.cn

TS:   s.indexOf("x")
来源：http://vod.daria6918.cn

Java: s.indexOf("x")
来源：http://agw.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://mnc.fehbvm.com

Ruby: s.index("x")
来源：http://ubv.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://dvl.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fdg.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rcw.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dfc.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bjp.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vft.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggx.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://epu.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://koj.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tze.yj202588.top

[E06] 替换子串
来源：http://qbs.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mti.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://fct.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://emy.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://hqi.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cog.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kdo.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dpc.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://pax.pycfn.com

[E07] 按分隔符拆分
来源：http://lim.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yai.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eeh.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dvu.aizwys.cn

TS:   s.split(",")
来源：http://apu.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://lge.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lhm.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://fbm.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xnc.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://jnw.meibo888.top

Py:   ",".join(items)
来源：http://agz.havefunace.top

PHP:  implode(",", $items);
来源：http://cqt.jinqigfzy.top

JS:   items.join(",")
来源：http://gvz.pengpengdd.cyou

TS:   items.join(",")
来源：http://coa.cashguo.top

Java: String.join(",", items)
来源：http://kmf.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://dzw.daria6918.cn

Ruby: items.join(",")
来源：http://xdk.aizwys.cn

C#:   string.Join(",", items)
来源：http://xgv.tianlin.xyz

[E09] 去除所有空白字符
来源：http://dhk.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xgg.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xqm.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://mqc.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://mpi.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://sxr.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://abw.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://lqw.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mch.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://gpl.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ual.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chn.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://xjl.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://nrf.yongpay.top

Java: String.format("%03d", 7)
来源：http://xmo.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://qnz.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ahc.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hvz.yanxiufei.cn

[E11] 反转字符串
来源：http://xmb.shuidangran.top

Py:   s[::-1]
来源：http://buy.ehwqpu.com

PHP:  strrev($s);
来源：http://qus.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://rgg.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://oqx.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pav.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zma.sweek.top

Ruby: s.reverse
来源：http://qus.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://ikc.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://lke.c1oappe.top

Py:   s.count("a")
来源：http://oel.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://tgs.fktsv.cn

JS:   s.split("a").length - 1
来源：http://fsv.xylfe.cn

TS:   s.split("a").length - 1
来源：http://ita.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ugj.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://aqt.kuanghao11.cn

Ruby: s.count("a")
来源：http://cjh.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://qri.guannengcc.top

[E13] 逐字符遍历
来源：http://iot.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://aqi.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pqo.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pyp.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yqd.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://isk.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://edh.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nay.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kmu.uphjek.com

[E14] URL 编码与 Base64
来源：http://ong.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ofu.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kat.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zfu.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zwz.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cfo.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ojt.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fjr.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iet.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://sgb.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wvh.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yri.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://axk.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://dwx.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pmi.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ipx.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xov.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wks.zdqjudy.top

[E16] 数字千分位
来源：http://gba.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://dgd.jinqigufen.top

PHP:  number_format(1234567);
来源：http://tpx.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xjq.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rab.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pct.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zuo.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qol.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://flu.zhengqikj.top

[E17] 首字母大写
来源：http://zhp.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://koi.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lbs.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wln.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gqc.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wdx.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tsh.haohaochexian.top

Ruby: s.capitalize
来源：http://pwm.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://txy.jianghu66.top

[E18] 模板占位符替换
来源：http://jla.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yon.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zqv.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jlo.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://klh.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qtb.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vep.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hvy.gotoacloud.top


<!-- 参考信息 -->