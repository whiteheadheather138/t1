代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gsrvhovkz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gqbiaozea.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzebavmt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.sjlbkw.cn/Article/details/gzroxfwdf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.epnwcf.com/Article/details/gbrgiuvco.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/gofrkeeir.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gdkbfyfln.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gihgvvkqd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.vehdjk.com/Article/details/gyquabycv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/grrqifcak.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gtwcimgby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/geswpoggy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gdfilvkub.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gbuxngtie.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gylsxufxp.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gtlpvompp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gdeqgzwea.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gskdmtrpw.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gyequlusr.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gzspuhbmo.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gproyehnv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gqruxxziw.sHtML

Ruby: arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gjjksfeng.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gdharppth.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/giqbbegmg.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gjayxscgt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmipnkhbm.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gsbkecctp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gsonesopn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gzlsnjewq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gochahtxr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gpdwiuvxr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gpaxhiavs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gtzfhemvg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gzzxaohgv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gckrmwmpz.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gmqcmvfaq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gkcdvbtiz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gjbhgfxxa.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gbtspbkoa.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gbgfoyqea.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gesykkooq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gtnxrvtpm.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gupgqvgeb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/ggqesbfpc.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gurnvwahf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/guhsfvqwt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gfssilkol.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gapcjwqlj.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gvogawzfs.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gmaimlzvn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gdrwpzqeq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gmprikorz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gjasmewsm.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gnharrorp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/grdsypzzt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gessyknwx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/guthxtawv.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gxkdwafjx.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gamadgsuy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gcmdfmcdc.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gwvkeemsq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gwsvsqocq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gmoqcentz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gwlyfjsjs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gwvzxjjlk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gvesnenky.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gxlvxxwbx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/geiiahmvm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gpwrcldju.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gpfdwvjfn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gsmoyahku.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gxxqcfrkj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gmvuyoyiz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gndcfbonl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gexqngvvl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gwmalamzu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/ghjzfuwfk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gxbrcwgyb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ggypwyxxw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfyftgqcu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gaqrivbjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gmpbmylwt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gjrtqcwge.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gdoqouwpg.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gpobabkkw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gcaunhmzr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/goomrzwgz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gzzccdqlp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/ghgditnjd.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.tarul.cn/Article/details/gckzxdwzj.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gofnczpao.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gtohdtxqi.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gppgitjrg.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/geaivjefw.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/goxmvutmn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gjovclvmm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gvksqxtwx.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/ggedcsqns.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gyvlbpaoe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gokfhoybq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gpczplvwd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/goewwwyyo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gphlsfpam.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/grqiqmjlz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/gdjvzwkxy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gxctkztfs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gdrlsxdwr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gkqhstysh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/guduknoug.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gdejttfty.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gygxnmhnn.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/guydwdnep.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gcqkyujvp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gbaetassa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gsscdxiyc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gpqmvqeub.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gawhvnsob.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/galltqxny.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqhqruvx.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/guqtphbpn.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gysebyeiq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/geftgayfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gjdqhvqek.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gwbjovgga.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gvnpnxlvm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gbgpzovrg.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gfhjkaugs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gxqutqljy.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/ggilwdgsp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/ghcnqtktm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gkztipwka.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/ghcfwreid.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gadelvdkf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gkxoqveas.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gokrrrtnz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gzxbibrsn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/gonmuukde.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/glddldfjk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/ggpcjdpyy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gkojopptn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gbrkdemde.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gkooqgwyg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gyldxmrfb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/glyoluuqp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/gtgvkzlro.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/ggncjefez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gdtazfeko.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gattplmue.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gxkczwgiz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gzgdwyejc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gxlvsqxxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/glxpkbpon.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/ggrugxoga.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.tarul.cn/Article/details/gyhrvnmai.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gbdvdxiao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gtduixuso.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/glmfltjdz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gnewawkre.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gfntufhou.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmmjcbiyh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gnowcinju.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gsqvmwkhp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gvbzbcxbn.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/ggwrvjyif.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gzifpkfhf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/glhkrgeru.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gctdzsldm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gkwsxrvht.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gikpqldkc.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gtnoxwjdl.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gzbvpytpz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gepggttqr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gqprysyro.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gimlovrpf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gyelttaae.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gkiytdquj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/geivaauwe.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gncqweiif.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gqbmfpcdq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/galznlnlg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/ggzxlapwo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/getnjjqna.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gpuskstrz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gnwojhhtr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gufthidqt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/ghqoyehqd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gxauefszg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/gbrljvifv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gwbevaait.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gpjsfbjjr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gactlgnag.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gbvfazdlo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gclxhpnum.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/guzxdxfsg.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gxsdpoeie.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gtedbkbxh.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gpwwgnpuy.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gkhuqqaay.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/ghrwpqhcv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gsqplaqyf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gnzzzpmqi.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gqxhpgywb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gtytodytr.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gidanqvnk.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gdyimsvwy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/ggeyzuufw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/glhzrszpc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gidiucuui.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gqjtxzpiz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gioopkxkl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrvogfgi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gvbiwleej.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gvwakcmpe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/giuvyypvp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/girjklxab.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gbaoihpcd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gjesmjagf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gujvgmiro.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/ggaucofxl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gfvsicjwv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gvtglkpxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gwpngcdhe.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/ghbhidock.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/grybjwwqm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpxgiwpjs.sHtML

F. 文件与目录
来源：http://read.share.sjlbkw.cn/Article/details/gnsrlehdn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqjbdddsi.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gflngpira.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gglysmxoc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqwblhgma.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gatixoncs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gmfwsjnhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/giqesnwpz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gnhfbilzo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gyzmyhuhk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gytlqroei.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/grnvsrihp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gvjcaansu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gacywpiig.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gzhxqxugq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gyhkjbtqy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gnehlribs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.sjlbkw.cn/Article/details/glzonhkxm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/grpirrayg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/ggpvmatsr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gbhcwfijl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gdfmogtab.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gumuwcqgk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gzipvkhvl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gwygfynqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gcbjvouzx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gvyrtjuhi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gznilzskl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/guxsdxdjn.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gtwjqaiqz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/grkexmbry.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gixqcrned.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gcelvvpiw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gxuqrxjvq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gurthnpus.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gjqgweoiz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/ggmtdihoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gvexfccfs.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gwrfhlqvr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gebshvlth.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/gxljkckmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gtpbjgtsh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyrdlgjdm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjkfulnr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/glpvyzxjd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gpawzquak.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gonufqgsa.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gzsksibvz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glecjqquz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gpqvkxnhn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gesirddnh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdaoyvonp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gtfxtetqq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfaxdscdi.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gsomvrqbx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqfebnatp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/grbdnmwwz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gmflefcvb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.vehdjk.com/Article/details/gjsryqgwn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gtxoeidbc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/ggzwhmdfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gcxudcjme.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gcsjecjbl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gcoossefw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gkeoueqal.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gutbzghfi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gqiauqyms.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/ghhprugrp.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gmyyhezmx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/glaidupqr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gkiivlmqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gjmihxpri.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gwitvihfr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/guwmfwjxn.sHtML


<!-- 参考信息 -->