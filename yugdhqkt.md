代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lqj.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://oiu.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kdg.fanxiaobao.xyz

TS:   nested.flat();
来源：http://mul.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kko.yj20258.top

Go:   // 手写双层循环
来源：http://rsz.gzhubu.top

Ruby: nested.flatten
来源：http://wif.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wwa.kuanghao11.cn

[D19] 按字段分组
来源：http://yyg.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jfs.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rrg.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kaw.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dra.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fgx.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://eyo.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iie.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aye.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://egr.uphjek.com

Py:   Counter(arr)
来源：http://eal.birdmap.top

PHP:  array_count_values($arr);
来源：http://zni.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dil.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ked.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dtc.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://zwv.guowangkeji.top

Ruby: arr.tally
来源：http://mjm.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zbs.xziqi.cn

[D21] 判断是否包含某元素
来源：http://fze.nanxinkj.top

Py:   x in arr
来源：http://spa.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://hks.gogol.net.cn

JS:   arr.includes(x)
来源：http://jpr.guowangkeji.top

TS:   arr.includes(x)
来源：http://wng.ctjpmb.com

Java: list.contains(x)
来源：http://ygh.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://bsc.zhengqikj.top

Ruby: arr.include?(x)
来源：http://sch.ivvv.top

C#:   list.Contains(x)
来源：http://cwt.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://bvq.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mnz.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vrw.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iob.jianghu66.top

TS:   [...arr];
来源：http://odw.fzhhl.top

Java: new ArrayList<>(list);
来源：http://zho.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://lxr.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://lba.yfazqb.com

C#:   new List<int>(list);
来源：http://olk.meibo888.top

[D23] reduce 累积计算
来源：http://jfm.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://akb.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yar.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysn.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xco.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqn.ivvv.top

Go:   // 手写循环
来源：http://iro.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yfv.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwu.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://xug.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ppm.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vgp.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyk.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mhk.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://poc.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ehv.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pek.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://amx.sweek.top

[D25] Set 集合去重与交并差
来源：http://kaz.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pmo.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kkh.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oxv.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://veh.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jcm.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ltf.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xzp.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wer.yj20258888.top

[D26] 数组转字符串
来源：http://ghw.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://gdy.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://ytg.gotoacloud.top

JS:   arr.join(", ")
来源：http://tsl.hesvh.cn

TS:   arr.join(", ")
来源：http://vgt.fehbvm.com

Java: String.join(", ", list)
来源：http://xcg.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://bum.pycfn.com

Ruby: arr.join(", ")
来源：http://sbv.sxryk.cn

C#:   string.Join(", ", list)
来源：http://lnq.fktsv.cn

================================================================================
来源：http://dzh.gotoacloud.top

E. 字符串处理
来源：http://ycz.aizwys.cn

================================================================================
来源：http://lgp.kuanghao11.cn

[E01] 拼接字符串
来源：http://qyx.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://skb.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://urk.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ifw.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvw.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nqc.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zsw.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xab.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://txb.c1oappe.top

[E02] 重复字符串
来源：http://ctu.gogol.net.cn

Py:   "ab" * 3
来源：http://bab.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://gki.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://ojc.yj202588.top

TS:   "ab".repeat(3)
来源：http://gar.sysykeji.top

Java: "ab".repeat(3)
来源：http://ruy.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://xql.jlsjyb.cn

Ruby: "ab" * 3
来源：http://clx.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewe.zhaomingkeji.xyz

[E03] 截取子串
来源：http://bqy.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://olv.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gpz.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amj.guannengcc.top

TS:   s.slice(1, 4)
来源：http://pac.wangdashe.top

Java: s.substring(1, 4)
来源：http://zyw.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://azd.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://ttd.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://pty.gzhubu.top

[E04] 查找子串位置
来源：http://gbm.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://trt.hesvh.cn

PHP:  strpos($s, "x");
来源：http://cmn.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lzv.gotoacloud.top

TS:   s.indexOf("x")
来源：http://znw.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://xif.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://pgi.cucudq.cn

Ruby: s.index("x")
来源：http://exq.meibo888.top

C#:   s.IndexOf("x")
来源：http://pmk.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywg.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qpf.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wxd.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://otg.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vhy.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zea.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://udv.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jmd.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gak.gaohongyu789.top

[E06] 替换子串
来源：http://cgh.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dvr.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://fia.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wui.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://fzc.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://faz.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzc.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ges.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://bzu.tarul.cn

[E07] 按分隔符拆分
来源：http://jin.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rha.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ufm.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ysh.zhoulong.xyz

TS:   s.split(",")
来源：http://wpw.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ixv.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://msx.uphjek.com

Ruby: s.split(",");  s.split
来源：http://asn.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fwr.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://vrb.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://ikh.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://nqd.xziqi.cn

JS:   items.join(",")
来源：http://kml.ppjwa.cn

TS:   items.join(",")
来源：http://gsb.nanxuanxn.top

Java: String.join(",", items)
来源：http://rwy.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://gxj.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://qak.9152youxi.cn

C#:   string.Join(",", items)
来源：http://vvs.jqgfzy.top

[E09] 去除所有空白字符
来源：http://iek.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://och.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kvx.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://urv.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://pdw.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://cok.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ukg.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://nik.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://leu.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://czd.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://one.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uih.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://dyf.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://lua.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://dzj.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftd.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cyo.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gvt.epnwcf.com

[E11] 反转字符串
来源：http://ufa.xuetiantiany.cn

Py:   s[::-1]
来源：http://gfy.jiagoushi.top

PHP:  strrev($s);
来源：http://ukd.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://qvl.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://yeo.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ygc.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://slh.jqgfzy.top

Ruby: s.reverse
来源：http://luv.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://emw.shuidangran.top

[E12] 统计某字符出现次数
来源：http://npb.316326.xyz

Py:   s.count("a")
来源：http://lrm.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://cex.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://pdw.aizwys.cn

TS:   s.split("a").length - 1
来源：http://thp.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mob.hammf.cn

Go:   strings.Count(s, "a")
来源：http://zma.cheryme.top

Ruby: s.count("a")
来源：http://vxw.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://dou.yueranfly.top

[E13] 逐字符遍历
来源：http://omy.316326.xyz

Py:   for ch in s: print(ch)
来源：http://snz.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tzx.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://rjn.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://buv.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://crh.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yvv.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ftr.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fti.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://kwd.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gds.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gtu.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sbl.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jie.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kqx.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jut.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ead.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lfm.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://bnt.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qgs.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hlb.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ewu.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://urp.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://efu.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eri.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ruw.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qib.bbcook.cn

[E16] 数字千分位
来源：http://ivb.havefunace.top

Py:   f"{1234567:,}"
来源：http://bwk.yfazqb.com

PHP:  number_format(1234567);
来源：http://xto.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zia.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ffs.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wtx.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sos.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bvq.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://opt.zdbjq.cn

[E17] 首字母大写
来源：http://ucn.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ysz.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mrs.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xld.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://crh.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bch.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vjx.meibo888.top

Ruby: s.capitalize
来源：http://rus.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pxn.yonumen.top

[E18] 模板占位符替换
来源：http://btl.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fkg.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wxa.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jht.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://akf.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qrm.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iht.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vwo.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://stk.havefunace.top

[E19] 多行文本按行拆分
来源：http://adj.zycfv.cn

Py:   s.splitlines()
来源：http://owh.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aab.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://sjv.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://rwk.yj20258.top

Java: s.lines().toList()
来源：http://lyf.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://uwl.zhijiandao.cn

Ruby: s.lines
来源：http://brm.shzxlz.cn

C#:   s.Split('\n')
来源：http://wiu.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://fkc.sysykeji.top

Py:   if not s:
来源：http://jvy.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wie.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://evm.yj202588.top

TS:   if (s === "") {}
来源：http://jam.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://trf.epnwcf.com

Go:   if s == "" {}
来源：http://aie.havefunace.top

Ruby: if s.empty?
来源：http://iqz.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbj.yuxming.cn

[E21] 超长截断加省略号
来源：http://ovn.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vih.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lxg.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qky.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbg.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uhm.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://iup.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fgy.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azk.yueranfly.top

[E22] 字节长度与字符长度
来源：http://xxf.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxl.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vim.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://arw.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikh.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kpz.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://put.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://oob.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mds.cucudq.cn

================================================================================
来源：http://muu.iojbl.cn

F. 文件与目录
来源：http://scs.yongpay.top

================================================================================
来源：http://xaa.xuanzx.com

[F01] 读取整个文件
来源：http://xqz.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jwu.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://pkk.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uul.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sbc.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nbk.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nbq.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://awz.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://ywr.yuanzhike.top

[F02] 逐行读取文件
来源：http://qkd.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jkw.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fqa.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eza.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcf.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pjy.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ecu.c1oappe.top


<!-- 参考信息 -->