代发 wailian999

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gnkntuurz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gbsyysyoc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gkhuizhpe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gcikcxicg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gzlhoamsy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gegbwdkcf.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gzfzbnpgq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gnwzcahiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/glwoddxxm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gorrdpnba.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/geyqovgpp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/ggmhkstgd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/grvexmqcq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gyeoqhucp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gwxvadrqp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gqdglcdad.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gvfaqpxej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/glwaqjzju.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/ghnvzmaro.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gxvowkjex.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gdpatqgvw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/guqmbpqlo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/ggilvbuas.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/ggjxsuvjr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gwoaalryt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnawiskak.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/glcklinrv.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gegzwwtnn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.bbcook.cn/Article/details/gkehhpgwg.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gosmefhxh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/giqpdomqf.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gcjhwzdbc.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gyuwbcuoc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gtzzjtyex.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gwvsovtqi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/guqrirpef.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbehyyxsm.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/geblxqyir.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtbbpdaul.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gjaojmkiv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/gedjnnlfm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gocclzwiy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gdbxljido.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/glrpculyz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gwrqwpgtu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/gidhbqciv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gsggudvom.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gihlzrjto.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gmaihnlqk.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gsqlhvaqt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gfinzwctn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/giyalqhrb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gvhxgqkqf.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gfgxbvftw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gwrnemcfa.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gqxjokitp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/grafqficj.sHtML

[E03] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gocyesivr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gdthdsetm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.tarul.cn/Article/details/guubmfcdm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gmllqkvva.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gtxnfkafo.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gaacfdluk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gbpgqwhwp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gwdympess.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gekhykxtu.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gugbxkygw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fktsv.cn/Article/details/gxxbnfxxe.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/gdnjbytho.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gxzcvakuo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ggpfnmpgj.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gpoelmmll.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gqavndfdf.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gqbuyliuh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gvqnbnqsk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fktsv.cn/Article/details/ghdzfabrb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gswztkdot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gymasgryc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gdygvspkn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gaazmiqmm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gtqmvqkzh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gfjukksyt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gaorlafiz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gzvfoxsjr.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/guoiaecal.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gdzyuyeuy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gzaeutzdk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gdmarzbzo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/grknnuinu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gifsiiury.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/grrawcjjs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gisnartlf.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gdobbmkpl.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/gydykwhsn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gnvqfenie.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gmkgjcrec.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gjpbycvje.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gmclfjiwk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gktvuzsku.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/gjesavunn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gdxxffqbi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gxymwahbl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/glepfkacg.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gfrxmnbfd.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gbrndycfy.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gidrpcbhc.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gitedcjna.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gvvwimfbl.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gzrwlomcz.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gbsixxxkr.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gwfiyahhd.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/grxknnong.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gdmyjhnua.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gcrtqnpbt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gipsiodlw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gmuioknnj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/ghnqtbzfc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gotgjxjfa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gjkahnjah.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gkqlzrxss.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gxjeoldcb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gwftjesje.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gczyxzaoy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gqijurpfv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gccbtggrf.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gilxidzxj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gqhpwfzjw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gqawhhgej.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gnvlvjacp.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/guqpvwssk.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gxxhomuil.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gyepeotda.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gxbeexswf.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gzetchnqo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gmlmeanyf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gqvewjasc.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gwyjqttmn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gwscipadt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gejxrsnjl.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gvybonqza.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gcdticzfg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gwupvjkas.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gxoptqwwp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gnuyejgph.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gjdsrbypw.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/giscpxngm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gwhouifiv.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdoztuwc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gceeetfpm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gfvumcyqw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/grefwednm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gjktrppfg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gbnqesybg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gtflgfspm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/glmhpkdzf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/grcwktwji.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/grvvlnqxy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gxjooylaq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gezohtjbx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/grkghqkfz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/ggozyqufw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gkpagfpdz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gnqvizuwh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/gonaneqvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/ghyyoxznd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/geymahfif.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gjfeehupo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.bbcook.cn/Article/details/gxuosopbt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gcknofnzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/gctbdmipb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gzdcbrxhc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/ggquwmvip.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrjwsnmo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gnpamfrgw.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gcdjufljv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/geqpgdehk.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gwqwrldzp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gptjbbbae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gaveewkil.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/guitpwzda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gvztvoyuk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gdodjotuo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gsokqyytc.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/guhhvndof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/goiqremer.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gsrbyrxap.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gmiblmcoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gxlvuzutw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gdumcholm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gklcigohj.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gtvrebzyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gknorxbzk.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gzypldyeh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gdxazzgsz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gcanfhwim.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gcoacjutj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gdvvblsim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gzccyqkui.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gkzexhmic.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gvnyhmqew.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/goabpvunr.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gjvpluurm.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gtrtdeqfv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ghqspboti.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gwvobcctt.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/geunxphvi.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gkixsuhka.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gatptrzhp.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gptxpfoic.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/gmoeaouqp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gaqsfxktk.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gdpabzjqm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/ggnqvhhzn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/glnonytpe.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gpciarmij.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gpnqqcpdm.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gzfvamnvr.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/goxqhctei.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvrzhsiqo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gmlcbwjed.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gsmegnubt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gwvzagbhi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gmhfgpuex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gbajvjbnm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/glrqtjyrd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gjojroclj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gmwxxptjf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gyhjqooty.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gqfsxaeue.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gawttgvyb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gwgnxpvsz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gqemslfev.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gzsqfjtnh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gmmcirqqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gyehsqtry.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gjumbzjfk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gyhuyhunu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gilrpmgia.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gsbohbogv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gorzwhhpr.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/gnmxfekps.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gxryizgcc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gtnjqdzdf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gcxgfztun.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/ggwusezpg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gxaeafmko.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/gjxmlylvo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkdihmcax.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grnhuwqsc.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gujockakz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gjdqffdmx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/gtxdipksi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gexpvskdk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpyvodoqq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gukhynbau.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/gjlrliznh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/grtcfctaz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/ggfyruopc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gppfjrmgy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gnamrebih.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gildsmehk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/grhllawvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gqhknigmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gbjnfxcso.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gcfmmfjco.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gixdjknbu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gguvuxvdo.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gfdeldcfm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gpfkkdsyh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gcrdjbbdb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/ggzzklypr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gvwechcrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gkddiuaud.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gjdiiefiw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gwhxiznzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gvsvafboy.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gkkiomobp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gaspyvupg.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/greepdwux.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/ghhusthmd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gshcfaifh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/glwpuuxrt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gsmvbfdob.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gdnptamnw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/goglhuicz.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/guwxopmax.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gadqwbakd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gcgdyarzo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/glqkjitlz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdrkndsjz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/grwhnapmf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gismwdecy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkpmqqraq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gmqsdylgt.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gspvsdisv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gensxknhs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gmepebgzc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gmrkxmesu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gjwyuvvmw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gmnvddkli.sHtML


<!-- 参考信息 -->