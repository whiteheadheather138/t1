代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://oic.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://okl.c1oappe.top

TS:   Math.max(...arr);
来源：http://mhb.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fsa.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cja.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://jxl.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://etm.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://vpd.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sdq.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://wvw.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xpf.gogol.net.cn

TS:   nested.flat();
来源：http://iow.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fye.hesvh.cn

Go:   // 手写双层循环
来源：http://xhw.jinqigufen.top

Ruby: nested.flatten
来源：http://kkt.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://btq.gzhubu.top

[D19] 按字段分组
来源：http://ttd.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://igk.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vlz.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jgs.tianlin.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://fle.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://orh.birdmap.top

Go:   // 手写 map[string][]T
来源：http://ohu.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://wpe.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bvw.havefunace.top

[D20] 统计每个元素出现次数
来源：http://dbu.yvedp.cn

Py:   Counter(arr)
来源：http://otm.c1oappe.top

PHP:  array_count_values($arr);
来源：http://dxo.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eeu.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lhy.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gdg.mhx1999.top

Go:   // 手写 map[T]int
来源：http://gca.zycfv.cn

Ruby: arr.tally
来源：http://utr.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wml.sweek.top

[D21] 判断是否包含某元素
来源：http://xvb.ydjk.org.cn

Py:   x in arr
来源：http://xkx.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://xio.jinqigfzy.top

JS:   arr.includes(x)
来源：http://yox.sufxvd.cn

TS:   arr.includes(x)
来源：http://vrn.hfpthk.cn

Java: list.contains(x)
来源：http://uax.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://umc.pycfn.com

Ruby: arr.include?(x)
来源：http://phe.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://grn.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://efo.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xvc.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nfu.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hps.yanxiufei.cn

TS:   [...arr];
来源：http://jbz.fzhhl.top

Java: new ArrayList<>(list);
来源：http://hzw.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://zgk.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://xnd.hammf.cn

C#:   new List<int>(list);
来源：http://vhb.xuanzx.com

[D23] reduce 累积计算
来源：http://bhh.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jqy.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqm.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vox.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zop.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://orx.zycfv.cn

Go:   // 手写循环
来源：http://rzv.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://csv.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wyh.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://afb.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qnv.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cwc.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://opc.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bqn.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lpa.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://osl.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yzr.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vkf.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://egu.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wdf.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sko.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkh.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nwr.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://khs.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://err.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezt.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ewa.jlsjyb.cn

[D26] 数组转字符串
来源：http://kfr.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://rqr.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://qhh.cashguo.top

JS:   arr.join(", ")
来源：http://ptb.tarul.cn

TS:   arr.join(", ")
来源：http://kki.fengsongda.top

Java: String.join(", ", list)
来源：http://fei.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://taf.meibo888.top

Ruby: arr.join(", ")
来源：http://qgy.cashguo.top

C#:   string.Join(", ", list)
来源：http://ict.vehdjk.com

================================================================================
来源：http://fth.guowangkeji.top

E. 字符串处理
来源：http://jnq.hesvh.cn

================================================================================
来源：http://vrs.nanxinkj.top

[E01] 拼接字符串
来源：http://mnn.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tvk.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tqz.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dmk.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://klz.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uah.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vly.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gbi.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mpe.yangfankeji.com

[E02] 重复字符串
来源：http://rre.316326.xyz

Py:   "ab" * 3
来源：http://hdv.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://txz.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://zpm.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://utl.nwbrower.top

Java: "ab".repeat(3)
来源：http://bqn.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://xyz.sysykeji.top

Ruby: "ab" * 3
来源：http://wuh.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hkx.bjfxy.top

[E03] 截取子串
来源：http://bqy.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eis.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://azu.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zcb.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://yqd.wangdashe.top

Java: s.substring(1, 4)
来源：http://ops.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cxt.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://euv.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://cfq.wangdashe.top

[E04] 查找子串位置
来源：http://tnd.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://wvc.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://gij.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fju.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://iqj.aibaodan.cn

Java: s.indexOf("x")
来源：http://gos.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://xaz.c1oappe.top

Ruby: s.index("x")
来源：http://ets.c1oappe.top

C#:   s.IndexOf("x")
来源：http://rdl.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hyl.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dhx.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zwt.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwe.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gix.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zhq.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://etn.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yai.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://orf.guowangkeji.top

[E06] 替换子串
来源：http://ivw.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgi.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://riw.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzm.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://jyd.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rvo.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://asl.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://npg.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://ckp.bbcook.cn

[E07] 按分隔符拆分
来源：http://eji.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tbs.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kpc.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dvt.gaohongyu789.top

TS:   s.split(",")
来源：http://mck.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://vau.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gfi.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://efd.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nzb.yj20258.top

[E08] 数组按分隔符合并
来源：http://sle.cdnleiting.top

Py:   ",".join(items)
来源：http://pwo.fzhhl.top

PHP:  implode(",", $items);
来源：http://pzz.xinyue.icu

JS:   items.join(",")
来源：http://flz.yj20258.top

TS:   items.join(",")
来源：http://wdc.shuidangran.top

Java: String.join(",", items)
来源：http://gew.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://dxn.yueranfly.top

Ruby: items.join(",")
来源：http://tqy.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://bgm.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://bhk.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blh.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://feo.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://pvy.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://bxn.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://otf.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://til.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://noy.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xgr.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://oss.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hdd.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dwn.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://gqe.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://kea.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://yne.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nht.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fgz.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eeb.hywenlv.cn

[E11] 反转字符串
来源：http://bxu.ydzc1.top

Py:   s[::-1]
来源：http://qct.zdqjudy.top

PHP:  strrev($s);
来源：http://jwv.316326.xyz

JS:   [...s].reverse().join("")
来源：http://ins.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://vnf.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://swi.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://xnb.iojbl.cn

Ruby: s.reverse
来源：http://wlp.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://bys.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://fnb.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://xzi.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://zzp.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://lmv.mhx1999.top

TS:   s.split("a").length - 1
来源：http://hou.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyl.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://abu.haohaochexian.top

Ruby: s.count("a")
来源：http://aau.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://qic.nanxuanxn.top

[E13] 逐字符遍历
来源：http://slc.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://iqk.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mxy.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fmy.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftl.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xql.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yek.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wzn.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://idr.iojbl.cn

[E14] URL 编码与 Base64
来源：http://tot.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ikw.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://qqa.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://izb.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://run.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pyw.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pja.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjm.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://amf.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://mgo.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://weq.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xei.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://phb.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://raa.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gft.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://utb.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ytw.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jld.zhoulong.xyz

[E16] 数字千分位
来源：http://oav.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://jjw.birdmap.top

PHP:  number_format(1234567);
来源：http://mtj.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bzi.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://atl.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://acw.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cri.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rex.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://lvh.havefunace.top

[E17] 首字母大写
来源：http://wuf.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xas.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mfw.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmh.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wiu.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xvi.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cos.9152youxi.cn

Ruby: s.capitalize
来源：http://kyc.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwg.snrcjt.cn

[E18] 模板占位符替换
来源：http://rzj.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gea.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ksv.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tmi.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nwd.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ykj.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ipi.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xke.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yiw.yfazqb.com

[E19] 多行文本按行拆分
来源：http://okw.gogol.net.cn

Py:   s.splitlines()
来源：http://odw.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kcw.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://xsb.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://ner.tian-w.cn

Java: s.lines().toList()
来源：http://arv.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://tvp.hcnkem.com

Ruby: s.lines
来源：http://xbz.aibaodan.cn

C#:   s.Split('\n')
来源：http://dbv.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://mza.316326.xyz

Py:   if not s:
来源：http://bgh.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bxl.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cgg.shuidangran.top

TS:   if (s === "") {}
来源：http://scp.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://zbq.feifeiyinyue.top

Go:   if s == "" {}
来源：http://xiw.jyoumei.cn

Ruby: if s.empty?
来源：http://hcm.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vrl.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://hkw.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nrl.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://haq.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://knh.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyw.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mvr.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://kxg.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://slj.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vum.epnwcf.com

[E22] 字节长度与字符长度
来源：http://bxv.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zhw.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wos.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lwa.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://txy.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dai.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zns.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://byf.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqb.zhongyouzk.top

================================================================================
来源：http://mdc.nanxuanxn.top

F. 文件与目录
来源：http://akc.zhengqikj.top

================================================================================
来源：http://wzd.hammf.cn

[F01] 读取整个文件
来源：http://ovf.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jka.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://pfy.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qfb.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ikq.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dam.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://knj.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://fdg.ivvv.top


<!-- 参考信息 -->