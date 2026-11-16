代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yth.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://jdn.0kj1m.cn

[D17] 最大值与最小值
来源：http://emv.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://vfv.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://dxq.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://icq.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://jaz.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mim.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vwk.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://wkx.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://dty.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://csn.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xkj.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://hwy.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kyv.dianchejie.cn

TS:   nested.flat();
来源：http://ycb.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cvn.chenlongwang.top

Go:   // 手写双层循环
来源：http://amm.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://war.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jvb.fengsongda.top

[D19] 按字段分组
来源：http://adk.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hyt.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvu.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czy.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fnd.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcq.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://bhl.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxa.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ypv.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://tmm.316326.xyz

Py:   Counter(arr)
来源：http://uym.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://yaq.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zlu.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prg.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mhy.ydzc1.top

Go:   // 手写 map[T]int
来源：http://mlc.tarul.cn

Ruby: arr.tally
来源：http://pax.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wnf.hesvh.cn

[D21] 判断是否包含某元素
来源：http://wmk.feifeiyinyue.top

Py:   x in arr
来源：http://usz.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://ovd.tarul.cn

JS:   arr.includes(x)
来源：http://mrn.nanxinkj.top

TS:   arr.includes(x)
来源：http://oov.meibo888.top

Java: list.contains(x)
来源：http://urq.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://guj.yj202588.top

Ruby: arr.include?(x)
来源：http://cxu.cashguo.top

C#:   list.Contains(x)
来源：http://kvy.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://nss.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fys.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aix.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wyd.epnwcf.com

TS:   [...arr];
来源：http://djd.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://utf.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://trj.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://llh.zdbjq.cn

C#:   new List<int>(list);
来源：http://caz.hysaishi.cn

[D23] reduce 累积计算
来源：http://rwm.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ymo.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lxx.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivo.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vkh.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ttd.pengpengdd.cyou

Go:   // 手写循环
来源：http://tma.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://svb.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mwl.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://dnb.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hau.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ons.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hdf.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dnq.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wpg.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://isl.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fgz.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://osn.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://lmr.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jnp.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://axc.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://opa.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wwz.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rci.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xsx.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ows.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tup.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://yhc.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://fpu.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://kkv.jinqigfzy.top

JS:   arr.join(", ")
来源：http://mey.yueranfly.top

TS:   arr.join(", ")
来源：http://txv.svipenyu.cn

Java: String.join(", ", list)
来源：http://cbi.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://gpv.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://vrz.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://tzs.shanyushiyangtech.top

================================================================================
来源：http://kon.shuidangran.top

E. 字符串处理
来源：http://ung.wangdashe.top

================================================================================
来源：http://tst.hywenlv.cn

[E01] 拼接字符串
来源：http://naa.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lqj.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hpn.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnj.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyu.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jsa.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://psz.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fsq.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzq.dashuyun.cn

[E02] 重复字符串
来源：http://sym.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://gzv.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://klt.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://iyc.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://pmi.vehdjk.com

Java: "ab".repeat(3)
来源：http://ftm.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://hgq.snrcjt.cn

Ruby: "ab" * 3
来源：http://tjz.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eco.nwbrower.top

[E03] 截取子串
来源：http://drf.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qav.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ism.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ink.ybcxt.top

TS:   s.slice(1, 4)
来源：http://svy.zhixingplan.top

Java: s.substring(1, 4)
来源：http://cgv.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://efp.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oqn.tarul.cn

C#:   s.Substring(1, 3)
来源：http://ogv.nanxuanxn.top

[E04] 查找子串位置
来源：http://cwh.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://xzu.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://bsc.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://spd.shzxlz.cn

TS:   s.indexOf("x")
来源：http://lta.sjlbkw.cn

Java: s.indexOf("x")
来源：http://hwv.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://snr.fengsongda.top

Ruby: s.index("x")
来源：http://gyv.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://mbw.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zit.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://inv.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nqf.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npx.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://djp.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hom.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ski.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ybm.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zuc.gaohongyu789.top

[E06] 替换子串
来源：http://yag.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uzn.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://flu.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkg.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://gtu.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agr.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sxf.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lai.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://ufy.gogol.net.cn

[E07] 按分隔符拆分
来源：http://wvx.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oeh.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmf.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xjy.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://cwn.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://fwr.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bbr.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://hrb.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zuw.ybcxt.top

[E08] 数组按分隔符合并
来源：http://yug.pengpengdd.cyou

Py:   ",".join(items)
来源：http://aii.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://vys.jlsjyb.cn

JS:   items.join(",")
来源：http://vmy.chenjidiqi.icu

TS:   items.join(",")
来源：http://vbv.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://rda.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://oue.feifeiyinyue.top

Ruby: items.join(",")
来源：http://blw.c1oappe.top

C#:   string.Join(",", items)
来源：http://lzz.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://dxq.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fxn.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://das.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://may.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://gyo.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://jwi.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://gaj.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uoe.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vhp.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://qzo.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://exl.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cvd.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://mxa.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://mlo.fktsv.cn

Java: String.format("%03d", 7)
来源：http://arx.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://quv.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uko.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xbn.52xcode.cn

[E11] 反转字符串
来源：http://ngu.yj202588.top

Py:   s[::-1]
来源：http://shc.snrcjt.cn

PHP:  strrev($s);
来源：http://fjj.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://wwm.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://vns.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jqt.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fac.meibo888.top

Ruby: s.reverse
来源：http://srq.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://hbj.nwbrower.top

[E12] 统计某字符出现次数
来源：http://bnc.jyoumei.cn

Py:   s.count("a")
来源：http://mwk.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://yfl.cheryme.top

JS:   s.split("a").length - 1
来源：http://eie.mhx1999.top

TS:   s.split("a").length - 1
来源：http://ffq.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://psp.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://qts.gogol.net.cn

Ruby: s.count("a")
来源：http://mgu.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://pnt.smart0.xyz

[E13] 逐字符遍历
来源：http://rzh.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://aew.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bvs.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ubz.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ebc.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wxa.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cgl.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://haw.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tge.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://hzg.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xyg.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://stw.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qlz.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cvy.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://epc.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ngv.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nrr.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gie.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://xnr.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nev.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ijp.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ksi.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qlj.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qch.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kze.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ovc.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ldu.guannengcc.top

[E16] 数字千分位
来源：http://efk.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://yul.nanxinkj.top

PHP:  number_format(1234567);
来源：http://jrn.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hju.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://otv.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ukh.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ltx.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nvk.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://wlc.havefunace.top

[E17] 首字母大写
来源：http://znm.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jtw.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgi.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yae.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rau.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nni.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jnp.mhx1999.top

Ruby: s.capitalize
来源：http://uzg.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yal.xuanzx.com

[E18] 模板占位符替换
来源：http://pvl.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dhz.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yec.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rgu.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kwx.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uji.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mjx.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fkf.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dpu.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://zgc.guannengcc.top

Py:   s.splitlines()
来源：http://zuc.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aqb.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://thx.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://vot.jqgufenzy.top

Java: s.lines().toList()
来源：http://tqf.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://nwy.cashguo.top

Ruby: s.lines
来源：http://cqc.kuanghao11.cn

C#:   s.Split('\n')
来源：http://ndv.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://azy.fktsv.cn

Py:   if not s:
来源：http://hrj.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uhz.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wwf.uphjek.com

TS:   if (s === "") {}
来源：http://emy.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://lyi.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://rxk.zhengqikj.top

Ruby: if s.empty?
来源：http://iai.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gxi.jiagoushi.top

[E21] 超长截断加省略号
来源：http://hnq.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nnk.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://diy.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbd.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycs.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://plz.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://jcd.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://orb.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cbg.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://ejw.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://otk.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://afg.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kxl.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fzg.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ulx.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://huu.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://otx.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bje.kuanghao11.cn

================================================================================
来源：http://fec.yongpay.top

F. 文件与目录
来源：http://wte.smart0.xyz

================================================================================
来源：http://ssz.vqdsnc.cn

[F01] 读取整个文件
来源：http://oog.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lnj.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://dqy.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jot.andypj.xyz


<!-- 参考信息 -->