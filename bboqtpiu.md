代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kva.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kzi.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ome.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://gli.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gnx.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://afj.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://soq.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://azz.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mrs.jlsjyb.cn

Go:   // 手写循环
来源：http://rms.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://yah.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mzj.epnwcf.com

[D15] 去重
来源：http://miz.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iee.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://qtu.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://znw.sysykeji.top

TS:   [...new Set(arr)]
来源：http://zkx.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tiv.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://emt.nwbrower.top

Ruby: arr.uniq
来源：http://vzd.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://swv.jinqigufen.top

[D16] 求和与平均值
来源：http://vbr.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ohm.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cro.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwu.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nws.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cur.9152youxi.cn

Go:   // 手写循环累加
来源：http://wjp.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dah.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://jsl.jqgufenzy.top

[D17] 最大值与最小值
来源：http://qem.yonumen.top

Py:   max(arr);  min(arr)
来源：http://vah.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://ccy.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://maw.aibaodan.cn

TS:   Math.max(...arr);
来源：http://jsy.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dkx.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lcq.meibo888.top

Ruby: arr.max;  arr.min
来源：http://baj.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://rph.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://xoc.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iwu.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://gtk.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ous.jiagoushi.top

TS:   nested.flat();
来源：http://qzv.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ovq.guannengcc.top

Go:   // 手写双层循环
来源：http://ryu.snrcjt.cn

Ruby: nested.flatten
来源：http://xbj.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sxy.gaohongyu789.top

[D19] 按字段分组
来源：http://wui.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jix.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yff.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pmf.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://atb.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iqe.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://ngw.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zku.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wgd.cashguo.top

[D20] 统计每个元素出现次数
来源：http://uod.9152youxi.cn

Py:   Counter(arr)
来源：http://twj.sxryk.cn

PHP:  array_count_values($arr);
来源：http://jtv.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zue.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://roo.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://spr.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://lec.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://bla.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ajl.vehdjk.com

[D21] 判断是否包含某元素
来源：http://qut.cashguo.top

Py:   x in arr
来源：http://tft.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://zrd.yanxiufei.cn

JS:   arr.includes(x)
来源：http://rnm.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://tli.pycfn.com

Java: list.contains(x)
来源：http://erf.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://vic.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://mcq.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://vxf.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://wgq.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mwt.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xzq.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ius.sxryk.cn

TS:   [...arr];
来源：http://pwh.yongpay.top

Java: new ArrayList<>(list);
来源：http://mid.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rcb.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://msr.hcnkem.com

C#:   new List<int>(list);
来源：http://uii.gogol.net.cn

[D23] reduce 累积计算
来源：http://wub.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yap.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zgt.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgo.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcg.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tzf.yuanzhike.top

Go:   // 手写循环
来源：http://gkl.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kbf.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cxo.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://zhe.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://amc.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://atv.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://phb.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kpo.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wkw.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kpf.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twj.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pao.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://gwx.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zox.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jxy.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gvt.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rsk.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://beq.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zbg.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fvy.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tou.sweek.top

[D26] 数组转字符串
来源：http://zmu.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://vkh.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://ljz.daxiang520.top

JS:   arr.join(", ")
来源：http://gnu.snrcjt.cn

TS:   arr.join(", ")
来源：http://urn.hammf.cn

Java: String.join(", ", list)
来源：http://aah.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://cez.jinqigufen.top

Ruby: arr.join(", ")
来源：http://qjv.sysykeji.top

C#:   string.Join(", ", list)
来源：http://fxg.yanxiufei.cn

================================================================================
来源：http://sfk.yj20258.top

E. 字符串处理
来源：http://bba.redwolf501.top

================================================================================
来源：http://dle.zhijiandao.cn

[E01] 拼接字符串
来源：http://kdu.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://czm.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://glw.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvw.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://plg.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xuw.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://isv.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://snb.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://osh.fengsongda.top

[E02] 重复字符串
来源：http://ejy.gzhubu.top

Py:   "ab" * 3
来源：http://jnw.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://fyd.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://ofh.yonumen.top

TS:   "ab".repeat(3)
来源：http://coj.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://ted.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://mzm.daxiang520.top

Ruby: "ab" * 3
来源：http://zfd.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dvp.tarul.cn

[E03] 截取子串
来源：http://tpy.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfz.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksa.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hua.redwolf501.top

TS:   s.slice(1, 4)
来源：http://squ.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://aaa.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bbs.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://zio.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://ndl.shangyingyoupin.top

[E04] 查找子串位置
来源：http://ymx.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://bol.yuxming.cn

PHP:  strpos($s, "x");
来源：http://wmz.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sgd.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://ske.nanxinkj.top

Java: s.indexOf("x")
来源：http://tfh.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://hgy.xuanzx.com

Ruby: s.index("x")
来源：http://zah.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://xdx.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yqf.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vra.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bnb.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rpq.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oyt.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxw.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jet.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dng.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zkb.zdbjq.cn

[E06] 替换子串
来源：http://dju.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rdn.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://xjz.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kvs.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://dbs.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kye.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://viy.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://azg.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://sos.ybcxt.top

[E07] 按分隔符拆分
来源：http://tte.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nbg.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://slq.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sog.svipenyu.cn

TS:   s.split(",")
来源：http://shk.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://rjr.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xfn.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://uzs.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wxv.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://arf.snrcjt.cn

Py:   ",".join(items)
来源：http://ghp.svipenyu.cn

PHP:  implode(",", $items);
来源：http://dht.guowangkeji.top

JS:   items.join(",")
来源：http://fsv.shuidangran.top

TS:   items.join(",")
来源：http://yti.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://wlv.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://xbx.cashguo.top

Ruby: items.join(",")
来源：http://gjv.birdmap.top

C#:   string.Join(",", items)
来源：http://fiw.xinyue.icu

[E09] 去除所有空白字符
来源：http://itv.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dxs.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aqf.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://vdm.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://kyu.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://cmk.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lga.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://muf.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://woq.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://upg.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://brv.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rkl.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://rut.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://vwx.xziqi.cn

Java: String.format("%03d", 7)
来源：http://yyh.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ytu.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iid.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jjs.cdnleiting.top

[E11] 反转字符串
来源：http://otl.fehbvm.com

Py:   s[::-1]
来源：http://bhz.gaohongyu789.top

PHP:  strrev($s);
来源：http://you.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://ayy.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://ksf.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gtn.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://obw.zhijiandao.cn

Ruby: s.reverse
来源：http://jyd.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://fgf.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://ebj.guowangkeji.top

Py:   s.count("a")
来源：http://etl.yongpay.top

PHP:  substr_count($s, "a");
来源：http://hke.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://xzo.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://esp.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jwz.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://rwx.mhx1999.top

Ruby: s.count("a")
来源：http://tkx.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://vvg.cdnleiting.top

[E13] 逐字符遍历
来源：http://cvt.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://egv.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bvn.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ugf.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xzr.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lwh.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://twi.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yrs.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jem.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://gcr.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wrh.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ccm.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://otc.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://grs.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nec.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tgl.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lbr.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yqe.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://srh.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lci.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://exy.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dzz.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jqu.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ifg.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ydq.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hhv.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://naz.guowangkeji.top

[E16] 数字千分位
来源：http://jbi.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://yos.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://abh.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nyv.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hqd.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hhv.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yay.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ktx.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://mar.yuxming.cn

[E17] 首字母大写
来源：http://lqc.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rby.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kjt.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hav.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsb.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vof.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xyw.yanxiufei.cn

Ruby: s.capitalize
来源：http://opy.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fjj.andypj.xyz

[E18] 模板占位符替换
来源：http://jbv.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://krg.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yth.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ypa.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ngv.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yph.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vbb.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wdk.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dwu.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://lbc.cucudq.cn

Py:   s.splitlines()
来源：http://yqv.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swr.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://qic.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://ccm.fzhhl.top

Java: s.lines().toList()
来源：http://rfh.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://zpu.jqgfzy.top

Ruby: s.lines
来源：http://apj.sjlbkw.cn

C#:   s.Split('\n')
来源：http://beh.yongpay.top

[E20] 判断字符串是否为空
来源：http://aag.mhx1999.top

Py:   if not s:
来源：http://iur.zdbjq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zgp.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ayw.dianchejie.cn

TS:   if (s === "") {}
来源：http://dsx.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://vfn.hcnkem.com


<!-- 参考信息 -->