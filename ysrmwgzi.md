代发 wailian999

[D19] 按字段分组
来源：http://doa.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uyd.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ojg.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vui.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyd.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dak.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://zzk.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qvo.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwa.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://kpk.chenlongwang.top

Py:   Counter(arr)
来源：http://mde.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://hwj.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blf.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kpq.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rgh.redwolf501.top

Go:   // 手写 map[T]int
来源：http://jdw.nanxinkj.top

Ruby: arr.tally
来源：http://qqz.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://how.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://rbr.hysaishi.cn

Py:   x in arr
来源：http://zzs.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://ddo.yuxming.cn

JS:   arr.includes(x)
来源：http://umj.sjlbkw.cn

TS:   arr.includes(x)
来源：http://uzr.hfpthk.cn

Java: list.contains(x)
来源：http://tuu.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://uzg.snrcjt.cn

Ruby: arr.include?(x)
来源：http://iqz.tianlin.xyz

C#:   list.Contains(x)
来源：http://wmm.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://igt.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wxf.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ddt.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hlw.xziqi.cn

TS:   [...arr];
来源：http://zax.guannengcc.top

Java: new ArrayList<>(list);
来源：http://qxd.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://gph.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://vxa.quarkkingdee.top

C#:   new List<int>(list);
来源：http://xid.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://uoy.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jay.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aum.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cba.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eoa.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wis.cashguo.top

Go:   // 手写循环
来源：http://exu.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://buk.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uve.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://jvz.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://meu.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sdv.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://paw.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kmg.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://esb.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zdm.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://win.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tsk.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://pbn.chenzaomai.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ipc.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nlw.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://csj.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zcu.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://shp.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ivk.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://coz.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fwe.zhongyouzk.top

[D26] 数组转字符串
来源：http://dbq.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://fbh.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://teb.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://mpe.sjlbkw.cn

TS:   arr.join(", ")
来源：http://toq.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://rwu.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://dou.gzhubu.top

Ruby: arr.join(", ")
来源：http://wyj.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://mzb.ydjk.org.cn

================================================================================
来源：http://zlf.xingfuxueyuan.xyz

E. 字符串处理
来源：http://hni.nanxinkj.top

================================================================================
来源：http://eaw.ydjk.org.cn

[E01] 拼接字符串
来源：http://krz.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plj.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dzb.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqi.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhv.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cad.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cqe.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wes.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qrb.hcnkem.com

[E02] 重复字符串
来源：http://npg.jinqigfzy.top

Py:   "ab" * 3
来源：http://tpy.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://uuo.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://tok.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://qrk.dashuyun.cn

Java: "ab".repeat(3)
来源：http://bcs.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://dml.c1oappe.top

Ruby: "ab" * 3
来源：http://qde.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dra.nanxinkj.top

[E03] 截取子串
来源：http://ljj.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://byp.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xyd.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eup.hcnkem.com

TS:   s.slice(1, 4)
来源：http://nju.gotoacloud.top

Java: s.substring(1, 4)
来源：http://glk.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fau.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://lsa.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://zyo.shangyingyoupin.top

[E04] 查找子串位置
来源：http://opi.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://nxj.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://npl.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gwy.hesvh.cn

TS:   s.indexOf("x")
来源：http://sko.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://ooa.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://szo.hongshengwenyu.top

Ruby: s.index("x")
来源：http://rjw.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://kof.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qoj.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hcp.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://djd.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zba.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zuv.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zwv.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yhl.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ujq.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jar.zhijiandao.cn

[E06] 替换子串
来源：http://jxx.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://imq.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vbw.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aca.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://vmh.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qss.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://txg.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zth.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://mac.gotoacloud.top

[E07] 按分隔符拆分
来源：http://jiz.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://leo.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qbk.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://djq.yonumen.top

TS:   s.split(",")
来源：http://ori.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://abt.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ybx.yj202588.top

Ruby: s.split(",");  s.split
来源：http://gzb.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gas.cucudq.cn

[E08] 数组按分隔符合并
来源：http://feq.aibaodan.cn

Py:   ",".join(items)
来源：http://zbd.hfpthk.cn

PHP:  implode(",", $items);
来源：http://agm.tianlin.xyz

JS:   items.join(",")
来源：http://mpn.gaohongyu789.top

TS:   items.join(",")
来源：http://jbj.cheryme.top

Java: String.join(",", items)
来源：http://npz.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://jmk.zhixingplan.top

Ruby: items.join(",")
来源：http://qss.havefunace.top

C#:   string.Join(",", items)
来源：http://zpw.cheryme.top

[E09] 去除所有空白字符
来源：http://zew.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ixn.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fls.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://rvj.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://yel.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://owr.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pym.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://ulu.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://foa.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://jgt.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nxi.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pzi.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://evi.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://mnp.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://ktb.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ayu.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jpb.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kxi.cucudq.cn

[E11] 反转字符串
来源：http://aum.gogol.net.cn

Py:   s[::-1]
来源：http://ile.svipenyu.cn

PHP:  strrev($s);
来源：http://jjb.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://xgv.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://qwr.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kgl.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://usg.zycfv.cn

Ruby: s.reverse
来源：http://dxi.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sjb.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://gol.xuetiantiany.cn

Py:   s.count("a")
来源：http://xmb.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://jil.ybcxt.top

JS:   s.split("a").length - 1
来源：http://dov.epnwcf.com

TS:   s.split("a").length - 1
来源：http://pww.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mde.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://qnk.jinqigufen.top

Ruby: s.count("a")
来源：http://ipn.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://wkl.hcnkem.com

[E13] 逐字符遍历
来源：http://unf.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://xnm.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dgc.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ugs.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://uzh.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://adp.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xoc.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yfb.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ffk.yj20258.top

[E14] URL 编码与 Base64
来源：http://gmf.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqk.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://drf.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dec.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ele.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gaq.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cdf.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pfx.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cax.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://jnb.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://qwm.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://atv.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ega.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ptv.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://his.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qib.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xca.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nyy.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://duf.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://nsp.zdqjudy.top

PHP:  number_format(1234567);
来源：http://atj.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yfn.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://krg.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eqi.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://toe.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kuz.uphjek.com

C#:   1234567.ToString("N0")
来源：http://wmz.yongpay.top

[E17] 首字母大写
来源：http://etm.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pmi.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aqv.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://igt.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hbp.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ygn.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ofi.zhengqikj.top

Ruby: s.capitalize
来源：http://usc.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://esz.hnxiangtu.top

[E18] 模板占位符替换
来源：http://xgm.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ubr.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mrs.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mvm.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hqg.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tdt.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jow.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cup.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qcb.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://nva.jiagoushi.top

Py:   s.splitlines()
来源：http://jvl.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vml.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://hcr.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://fwr.nanxuanxn.top

Java: s.lines().toList()
来源：http://ock.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://ltq.shzxlz.cn

Ruby: s.lines
来源：http://fmg.xinyue.icu

C#:   s.Split('\n')
来源：http://mkc.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://qaf.hcnkem.com

Py:   if not s:
来源：http://hxl.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rzt.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bus.hnqzz.top

TS:   if (s === "") {}
来源：http://olh.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://vnn.vehdjk.com

Go:   if s == "" {}
来源：http://irp.fehbvm.com

Ruby: if s.empty?
来源：http://jqa.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nye.yj20258.top

[E21] 超长截断加省略号
来源：http://ggz.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktj.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pko.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ukp.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obu.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fca.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ymx.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xtr.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfj.yj202588.top

[E22] 字节长度与字符长度
来源：http://eus.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rpb.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zkj.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://asa.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sqt.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ldz.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fpc.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://zmp.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fnv.xinyue.icu

================================================================================
来源：http://cos.zhijiandao.cn

F. 文件与目录
来源：http://fks.0kj1m.cn

================================================================================
来源：http://gnw.ppjwa.cn

[F01] 读取整个文件
来源：http://wtr.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://imb.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://ezx.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zqw.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ray.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sqk.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vih.daria6918.cn

Ruby: File.read("a.txt")
来源：http://hjs.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://zai.dianchejie.cn

[F02] 逐行读取文件
来源：http://wvj.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://frl.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bms.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgq.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dsj.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jde.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://brh.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vrv.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ntc.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://izw.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://txd.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cfk.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hjs.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzo.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://luk.feifeiyinyue.top


<!-- 参考信息 -->