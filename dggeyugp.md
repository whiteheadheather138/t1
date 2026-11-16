代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://glr.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kyt.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://abo.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://jwi.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://ceu.svipenyu.cn

Go:   // 手写循环
来源：http://mah.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zvy.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://chv.sweek.top

[D15] 去重
来源：http://zal.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pyb.shuidangran.top

PHP:  array_unique($arr);
来源：http://wso.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://hzl.yfazqb.com

TS:   [...new Set(arr)]
来源：http://iki.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vhz.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://imj.gzhubu.top

Ruby: arr.uniq
来源：http://bzw.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://qcj.zhongyouzk.top

[D16] 求和与平均值
来源：http://rsw.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nck.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rco.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cch.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iux.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bkt.jyoumei.cn

Go:   // 手写循环累加
来源：http://tmg.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://psf.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://ekh.sysykeji.top

[D17] 最大值与最小值
来源：http://qpe.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://ang.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://vrq.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ihn.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://lnj.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vmt.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bfb.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://dye.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://gpz.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://hal.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qew.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://xgn.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://msc.gotoacloud.top

TS:   nested.flat();
来源：http://bzj.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jjt.fehbvm.com

Go:   // 手写双层循环
来源：http://dua.pengpengdd.cyou

Ruby: nested.flatten
来源：http://wpi.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbn.vqdsnc.cn

[D19] 按字段分组
来源：http://igj.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gej.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kwy.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bvk.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zoi.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzb.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://zce.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://toe.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oep.ivvv.top

[D20] 统计每个元素出现次数
来源：http://hem.daria6918.cn

Py:   Counter(arr)
来源：http://xov.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://vly.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvm.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vkz.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yaa.birdmap.top

Go:   // 手写 map[T]int
来源：http://gkh.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://hlo.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bzl.redwolf501.top

[D21] 判断是否包含某元素
来源：http://lte.jianghu66.top

Py:   x in arr
来源：http://kpz.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://hhw.cdnleiting.top

JS:   arr.includes(x)
来源：http://wlu.uphjek.com

TS:   arr.includes(x)
来源：http://lzv.dianchejie.cn

Java: list.contains(x)
来源：http://pyw.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://yij.smart0.xyz

Ruby: arr.include?(x)
来源：http://yvr.52xcode.cn

C#:   list.Contains(x)
来源：http://rcd.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://gyo.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tkv.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wvt.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pol.hnxiangtu.top

TS:   [...arr];
来源：http://jju.52xcode.cn

Java: new ArrayList<>(list);
来源：http://tsy.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://jqr.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://hal.sysykeji.top

C#:   new List<int>(list);
来源：http://hjj.xziqi.cn

[D23] reduce 累积计算
来源：http://bhx.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phl.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zyi.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mgg.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ewk.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsa.tarul.cn

Go:   // 手写循环
来源：http://neq.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hkz.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mrd.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://wze.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ksd.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ull.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ghv.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fro.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hki.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mxb.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izq.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xpw.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://txp.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://seg.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jtl.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://erg.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wcj.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dck.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fat.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xye.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sad.gzhubu.top

[D26] 数组转字符串
来源：http://rvs.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://wne.havefunace.top

PHP:  implode(", ", $arr);
来源：http://kap.gotoacloud.top

JS:   arr.join(", ")
来源：http://vzf.dianchejie.cn

TS:   arr.join(", ")
来源：http://pqp.ehwqpu.com

Java: String.join(", ", list)
来源：http://oep.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://gch.sysykeji.top

Ruby: arr.join(", ")
来源：http://aqj.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://uws.jianghu66.top

================================================================================
来源：http://gmi.xylfe.cn

E. 字符串处理
来源：http://fwi.ywan-chungtsiang.top

================================================================================
来源：http://jfa.yueranfly.top

[E01] 拼接字符串
来源：http://elc.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eai.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zbo.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mey.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jvc.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gbh.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mfd.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://spt.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yun.yvedp.cn

[E02] 重复字符串
来源：http://zsb.yj20258888.top

Py:   "ab" * 3
来源：http://ngg.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://ssc.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://iid.hcnkem.com

TS:   "ab".repeat(3)
来源：http://xka.cashguo.top

Java: "ab".repeat(3)
来源：http://kte.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://hjl.redwolf501.top

Ruby: "ab" * 3
来源：http://lbd.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nnv.xziqi.cn

[E03] 截取子串
来源：http://ipv.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sxy.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yic.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tis.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://aac.aizwys.cn

Java: s.substring(1, 4)
来源：http://rtq.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ixp.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://otf.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://lhg.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://ece.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://jjq.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://nal.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vvf.sysykeji.top

TS:   s.indexOf("x")
来源：http://wxa.dashuyun.cn

Java: s.indexOf("x")
来源：http://ewz.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://xrb.9152youxi.cn

Ruby: s.index("x")
来源：http://aso.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://jbg.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://not.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lyt.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vpc.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rxb.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lfe.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djn.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zse.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vfd.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bxj.tian-w.cn

[E06] 替换子串
来源：http://opq.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvd.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://tqk.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qgt.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://fyf.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nup.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iem.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qre.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://avy.zycfv.cn

[E07] 按分隔符拆分
来源：http://xzd.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://szc.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://klm.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rwp.yj20258888.top

TS:   s.split(",")
来源：http://fhm.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://kbz.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://igt.sweek.top

Ruby: s.split(",");  s.split
来源：http://sjv.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wbr.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://ubk.jlsjyb.cn

Py:   ",".join(items)
来源：http://dcm.daxiang520.top

PHP:  implode(",", $items);
来源：http://ttw.yongpay.top

JS:   items.join(",")
来源：http://nbz.fehbvm.com

TS:   items.join(",")
来源：http://vxz.yj20258888.top

Java: String.join(",", items)
来源：http://hdk.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://xcw.316326.xyz

Ruby: items.join(",")
来源：http://lhn.havefunace.top

C#:   string.Join(",", items)
来源：http://pql.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://rzv.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fsk.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wts.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://mng.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://qqi.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://kxs.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wzc.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://ywc.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oxm.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://jik.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ern.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cqx.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://fky.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://sdi.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://egd.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jfm.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jxg.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lps.hongshengwenyu.top

[E11] 反转字符串
来源：http://tsi.ybcxt.top

Py:   s[::-1]
来源：http://lrk.hfpthk.cn

PHP:  strrev($s);
来源：http://sby.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://pmx.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://imf.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://las.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wpm.gzhubu.top

Ruby: s.reverse
来源：http://buu.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wgy.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://ior.jlsjyb.cn

Py:   s.count("a")
来源：http://fxd.meibo888.top

PHP:  substr_count($s, "a");
来源：http://bbf.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://qrt.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://uud.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rtb.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://bsu.smart0.xyz

Ruby: s.count("a")
来源：http://cir.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://jzw.chenlongwang.top

[E13] 逐字符遍历
来源：http://vte.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://hai.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tpd.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ipf.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ngo.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fjf.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wuh.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rbh.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kmn.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://pma.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wwz.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lci.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://err.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ahb.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xvu.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gau.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://evh.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jbg.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://szo.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://htu.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://crh.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aly.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://paf.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pmx.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mmj.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rlo.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wdy.bjfxy.top

[E16] 数字千分位
来源：http://jtm.andypj.xyz

Py:   f"{1234567:,}"
来源：http://zvk.cashguo.top

PHP:  number_format(1234567);
来源：http://ijq.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xeq.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jqy.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mxi.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://byo.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wcq.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://pdj.tianlin.xyz

[E17] 首字母大写
来源：http://sac.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qop.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://tcr.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyr.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fny.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fqb.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zxj.yongpay.top

Ruby: s.capitalize
来源：http://ews.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cjb.wangdashe.top

[E18] 模板占位符替换
来源：http://tgv.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mqo.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ikw.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lgv.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fuk.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uak.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpi.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://una.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vuk.sweek.top

[E19] 多行文本按行拆分
来源：http://srj.sysykeji.top

Py:   s.splitlines()
来源：http://bkr.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsu.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://nsh.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://lvn.zhijiandao.cn

Java: s.lines().toList()
来源：http://maz.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://bxs.hnxiangtu.top

Ruby: s.lines
来源：http://ayq.guannengcc.top

C#:   s.Split('\n')
来源：http://yus.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://tql.jiagoushi.top

Py:   if not s:
来源：http://our.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ede.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ftz.tarul.cn

TS:   if (s === "") {}
来源：http://cfo.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://tgc.aibaodan.cn

Go:   if s == "" {}
来源：http://ihv.zdqjudy.top

Ruby: if s.empty?
来源：http://udv.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uin.ehwqpu.com

[E21] 超长截断加省略号
来源：http://jbz.sysykeji.top


<!-- 参考信息 -->