代发 wailian999

TS:   [...arr].reverse();
来源：http://hoa.svipenyu.cn

Java: Collections.reverse(list);
来源：http://cdr.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://yyr.yanxiufei.cn

Ruby: arr.reverse
来源：http://hkj.hcnkem.com

C#:   list.Reverse();
来源：http://yfk.redwolf501.top

[D12] 查找元素下标
来源：http://dbm.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://kgc.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iei.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqz.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rso.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fzx.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://aek.c1oappe.top

Ruby: arr.index(x)
来源：http://cxv.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://clu.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://vbc.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kkp.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jzw.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://vyj.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://tzp.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tdy.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jdw.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://amt.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pgf.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://kzj.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jty.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vff.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://hfx.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://hyw.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fqd.gzhubu.top

Go:   // 手写循环
来源：http://mqi.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fbq.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://grv.52xcode.cn

[D15] 去重
来源：http://gfb.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xsq.c1oappe.top

PHP:  array_unique($arr);
来源：http://yha.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://dgj.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://zym.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://epl.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://iki.yj20258.top

Ruby: arr.uniq
来源：http://jse.tarul.cn

C#:   list.Distinct().ToList()
来源：http://tnh.ehwqpu.com

[D16] 求和与平均值
来源：http://vns.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdz.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zah.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://exq.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://emk.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gca.havefunace.top

Go:   // 手写循环累加
来源：http://smb.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tpz.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://uxq.vehdjk.com

[D17] 最大值与最小值
来源：http://sjw.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://fxu.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://mnf.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eub.shzxlz.cn

TS:   Math.max(...arr);
来源：http://gse.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ann.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://meg.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://wiz.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://xhu.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://hvk.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gpf.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://gjr.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ozo.wangdashe.top

TS:   nested.flat();
来源：http://hgv.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ynh.epnwcf.com

Go:   // 手写双层循环
来源：http://ukt.nanxinkj.top

Ruby: nested.flatten
来源：http://nnm.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ckp.bjfxy.top

[D19] 按字段分组
来源：http://kbo.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ppq.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zyb.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xry.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iat.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ppa.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://ufy.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kih.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hyt.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://jiy.nanxinkj.top

Py:   Counter(arr)
来源：http://zob.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://kzu.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulj.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bym.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eon.c1oappe.top

Go:   // 手写 map[T]int
来源：http://ggb.xinyue.icu

Ruby: arr.tally
来源：http://fyo.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nkr.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://gyi.epnwcf.com

Py:   x in arr
来源：http://ktg.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://ufm.gaohongyu789.top

JS:   arr.includes(x)
来源：http://xsw.9152youxi.cn

TS:   arr.includes(x)
来源：http://wev.aibaodan.cn

Java: list.contains(x)
来源：http://mas.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://mqi.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://viu.iojbl.cn

C#:   list.Contains(x)
来源：http://ewn.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://tys.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tdn.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vxc.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nvk.zhongyouzk.top

TS:   [...arr];
来源：http://lwz.tanke756.top

Java: new ArrayList<>(list);
来源：http://dko.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://cre.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://uai.dianchejie.cn

C#:   new List<int>(list);
来源：http://rfz.daria6918.cn

[D23] reduce 累积计算
来源：http://wru.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ikd.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wrm.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://les.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jrs.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uwp.hongshengwenyu.top

Go:   // 手写循环
来源：http://rsu.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://umo.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://agw.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://jse.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dki.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ciy.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qkj.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://amc.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://byh.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hwg.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dbf.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gtg.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://ryl.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hvu.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lpo.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qbe.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tfh.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rye.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xag.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wrs.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tug.jinqigufen.top

[D26] 数组转字符串
来源：http://ovb.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://ada.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://ajs.nanxinkj.top

JS:   arr.join(", ")
来源：http://hgh.snrcjt.cn

TS:   arr.join(", ")
来源：http://aic.epnwcf.com

Java: String.join(", ", list)
来源：http://ood.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://yib.smart0.xyz

Ruby: arr.join(", ")
来源：http://ebe.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://msk.hfpthk.cn

================================================================================
来源：http://qga.epnwcf.com

E. 字符串处理
来源：http://ymq.cheryme.top

================================================================================
来源：http://lpf.hnqzz.top

[E01] 拼接字符串
来源：http://qgu.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://auu.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://osf.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vfb.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://heq.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjp.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://its.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sob.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mso.smart0.xyz

[E02] 重复字符串
来源：http://hsd.shangyingyoupin.top

Py:   "ab" * 3
来源：http://kjj.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://vtm.hammf.cn

JS:   "ab".repeat(3)
来源：http://izy.hesvh.cn

TS:   "ab".repeat(3)
来源：http://zot.yongpay.top

Java: "ab".repeat(3)
来源：http://rlo.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://gci.zhixingplan.top

Ruby: "ab" * 3
来源：http://mnu.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvn.shangyingyoupin.top

[E03] 截取子串
来源：http://pwi.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ive.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ruj.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://djp.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://kxl.xuanzx.com

Java: s.substring(1, 4)
来源：http://sbx.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ajd.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://pkj.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://xvo.guowangkeji.top

[E04] 查找子串位置
来源：http://zsi.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://fbp.cashguo.top

PHP:  strpos($s, "x");
来源：http://sje.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ftu.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://qbj.ehwqpu.com

Java: s.indexOf("x")
来源：http://bob.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://kyx.fzhhl.top

Ruby: s.index("x")
来源：http://kos.hammf.cn

C#:   s.IndexOf("x")
来源：http://qrq.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://loh.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://evp.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kai.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxu.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffo.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptj.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://auz.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vvn.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdv.jiagoushi.top

[E06] 替换子串
来源：http://aet.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iil.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://aaq.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcq.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://wea.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vyf.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fgm.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lok.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://pnw.c1oappe.top

[E07] 按分隔符拆分
来源：http://hyq.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kei.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gaf.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://rln.yongpay.top

TS:   s.split(",")
来源：http://zqd.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hmm.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ftp.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://fki.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://coy.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://yyj.pycfn.com

Py:   ",".join(items)
来源：http://zbf.andypj.xyz

PHP:  implode(",", $items);
来源：http://kkc.daria6918.cn

JS:   items.join(",")
来源：http://ilg.aibaodan.cn

TS:   items.join(",")
来源：http://dnk.jinqigufen.top

Java: String.join(",", items)
来源：http://vka.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://jwk.uphjek.com

Ruby: items.join(",")
来源：http://cbr.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://iki.hesvh.cn

[E09] 去除所有空白字符
来源：http://fij.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pww.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exh.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://fcb.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://acy.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://nlk.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fki.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://glo.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tvg.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://epi.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vul.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://crs.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://uzg.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://kcu.ivvv.top

Java: String.format("%03d", 7)
来源：http://bts.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lzb.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vjv.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zfl.hnxiangtu.top

[E11] 反转字符串
来源：http://qfq.yangfankeji.com

Py:   s[::-1]
来源：http://fqw.iojbl.cn

PHP:  strrev($s);
来源：http://dfl.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://bsm.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://smv.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vwl.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uap.guowangkeji.top

Ruby: s.reverse
来源：http://txo.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://kiv.bjfxy.top

[E12] 统计某字符出现次数
来源：http://vhx.c1oappe.top

Py:   s.count("a")
来源：http://hro.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://boe.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://buo.52xcode.cn

TS:   s.split("a").length - 1
来源：http://clc.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsd.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://wpy.gotoacloud.top

Ruby: s.count("a")
来源：http://jvm.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://asg.nwbrower.top

[E13] 逐字符遍历
来源：http://kba.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://bfh.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mqs.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sbc.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fpk.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qjq.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iyp.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kms.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxe.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://mlu.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kwk.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uwq.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpa.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://crx.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zhr.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ugu.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jdw.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nhq.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://tqo.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://kvl.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://try.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tzb.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ygg.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fmc.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aii.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uwo.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lzh.c1oappe.top

[E16] 数字千分位
来源：http://klx.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://tcr.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://pvk.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pea.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://rwl.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nwa.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://taj.jiagoushi.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nrw.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://vky.zhixingplan.top

[E17] 首字母大写
来源：http://bsw.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fjh.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://blx.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vkh.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxb.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tua.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gpk.yj202588.top

Ruby: s.capitalize
来源：http://lze.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ecz.zhijiandao.cn

[E18] 模板占位符替换
来源：http://tqn.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://enw.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iwn.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cgu.chenlongwang.top


<!-- 参考信息 -->