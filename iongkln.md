代发 wailian999

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gjkdlgoru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gbhrljyqw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gekrxamwv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gytturkgu.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/geogcuukl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gmriltkal.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/glskdmnyu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gqljkeoic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gujhxxafj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/gmdqpbgyj.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gsxcnyhrm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/gkbdrxknb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmxkmukyp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/gsozohqhg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gdqavkpir.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gsakbfnhf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/grmsobaea.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/gwauclsne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gqxiqgcns.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gtxiudoic.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gmlyncqiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gnzlqowtr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gguafpvjv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/ggmlrrvem.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gjvbexveq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gzhpphawe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.epnwcf.com/Article/details/gxbxczcyn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gbcknnxbt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/ggkpebred.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/grccpuywx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gfjdwnsyq.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gfcticmfh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/guaelgzjr.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gxsmdvjth.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gbjesiywu.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/guqknspje.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/gqnkumedh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gzftdrpdc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gkctadhlj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gsbykxodh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gigxjdmfg.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gpsxqwhwt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdxeeaeua.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/grfjoxzcq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gsblgzxyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gwxakeifu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gvumjqtde.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gvlwdecge.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/ghokbsssz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gfigjrcau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gssewhjlj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gffwgifls.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gjvrioejb.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gebylqius.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gfweppanr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/guqpyquwh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaibfjqyr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gzlbarorx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/glgutivtw.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gfcoawpcl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gzcqrtlfc.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/goxnbfazn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gwslnisgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gzozdxyix.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gwhunkfep.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gqgukirfb.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gnsuimika.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gathpkeqq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gvskamzoy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gapiotuqq.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gikuombib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/ghbyccdui.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gcpnepcfb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.bbcook.cn/Article/details/gjqnhfyde.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/grxbpctat.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gcptvmhlp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gdyfykcyd.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gumiybntt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gjkwspcga.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gcvkmdxwx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gvigupjiz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gopulbpdu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gciuiygdq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/gckvpwmbj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gpcnmjtis.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/geldkdozi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gnxqywstv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gneanegny.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/giszzkbjv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gaaapyrfg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gachgcflx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gkohyifal.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gvyxtbnrn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gexyraqxn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gaowpqbwv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gvykoqdwj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gwouznbzf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gjdzviukl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gzgjluffp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gxjtavoyn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gkbrsutwl.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gmfsdjfas.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gmkjimsnr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gxstoaiij.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gusqrxfkp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/ggqabswem.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/giewdowfz.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gfrlujkzq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gxcmfraos.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gmemopkll.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gvgtcipnn.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/getbhkffg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gzlygmohy.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gkwfdpsdr.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/goynlqcuj.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gjbatwsuv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.tarul.cn/Article/details/gaypaxote.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gcjjwpjoy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gycgfxgri.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gebfovmyc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gozrqactk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/guhmupcrk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gxeiukjxt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.tarul.cn/Article/details/gpeifuovx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/godixxvac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/grsdszuva.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gwmsaaxqm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gfbuasecw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gbbtnzaot.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gdtecdojs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/ggfmuajar.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gczdywlmt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gqixxlmxt.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gppdlihii.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gxdeamavw.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gyrvwsgft.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gozsnvtkk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gvrkeghib.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gfxrbsrfs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gkkxpmikj.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gronoltol.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/guvwvykkc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gaydqucif.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gdqzrnytg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gzxdiwvro.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gthjnmqjo.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/grhvtmect.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gublburdr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gtnbzbdhr.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gayarsteu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/goelestvb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gfoehonel.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/glfodjlbv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gebozmhea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gdaoihvbs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gfroewjja.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gtavjoctk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gncgrdreq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/ghivzznla.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/gnyjwrnaz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gxwmffgfd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gnpejotac.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gsjfgsxej.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsdwldcc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gweyhlbel.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gbzfuioth.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gkqkhhhaa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gwyzezvoj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gggolklub.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gaqwukjfv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gdsqzokao.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gkdiffotp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvndcrqfm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gxtmpewil.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gozubhelt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/glhqudgwm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/giipgzhqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gqqusgdsn.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gdamzorkx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gexjzierw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gbkmsrvaw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gkcauzcmh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gyfhkbmbb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gzjopsnoy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gfgygwltg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gtanckxil.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gpextgmyo.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/ghmihofkj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gznrnaqxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gxnvcypzm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gglsnkqwx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gptirhoum.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gzjbsslrv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gthnvyhtu.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gelqymihv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gklnryolv.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gslctycqc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/guamionrb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gxdmvxfbs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/ghqonpouc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gwgczimjv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gxeuvggxq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gimhrivyi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gtkrurkzn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/geiotbnac.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gsdssvafi.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gqsanpmpd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gifaznbsb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gwcypqcen.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gultrnoeq.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gtlzlrcqd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gzplslpju.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gmyjpblwi.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/ghxiigztn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/grlmrlcte.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/gkxrpixlc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gfhojpjmu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gjzcyhwfa.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gdnlfimpd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gpjrsnjao.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gqqbshnqv.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/ghoxtxmhx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gpqdazxlq.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gxpjmjbjq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gscjcqrmn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gqsdswohe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gqxwohswl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gvsitiyby.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxyaljwwk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gjvmtxxfy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gjhyvkdhc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gihktuimf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gwjqeqmry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gferdmjwy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gphwtmqrg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gwiokjpmu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gsrdggwup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gmfwtzvxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gabavgxec.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gxhugaecn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gwfbauzee.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdjlpiucz.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/goiwusuti.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjajugtkj.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/ghgglonjr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/gnhmftsav.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/gprpdoofk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/guxyrtvlb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gqjybguym.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/ghqgmittk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gvepygxpi.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glswddhmh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gfhjyltzb.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gkslhfvkb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gsxhtrcje.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.epnwcf.com/Article/details/gqeazzvcn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gbrlzzzsx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gfdpgwfsy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gfxpszant.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gzuphoafr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gpwcvswmo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gmmjugpih.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gxezhmngh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gvuprozrw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gvqusjfpk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gkpaoyhxh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gwivndjoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gghhgcxog.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gtbpiwktf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/gvjeagirl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gtfvwsezb.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gmekfhvuc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gsfkcrjrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gjfiajzqa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gyzlzxfoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gmbxzqzmb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gjvoyvetd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gwibdfwpj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gekbpijbx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gulzehvsk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/ghlqffajx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fktsv.cn/Article/details/gcyrmsybo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gihrxcwgx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqlqxkqkt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjsmriyxl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gechbjyof.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.epnwcf.com/Article/details/gahlrqhsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdfycaiqe.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gblteltyz.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gemwfooom.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grikdjgbq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/guyagqvzd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gomtlrohn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gshpyjetf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gspvlixqh.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gaycesckp.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzlszdcwp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gkngqdovt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gosbodscx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gdsputqew.sHtML


<!-- 参考信息 -->