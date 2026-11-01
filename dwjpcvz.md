代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gwssfuykn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gffppnwoo.sHtML

C#:   list.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gboymvioc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/ggffunscm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gfumbjlre.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/glaptfvpw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gkkhlvuko.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gvyaryhkn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gqswgrhwm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/genrgepzf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/glmopyhdu.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/guvhtgyyv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gmhljnqdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gthntpdqf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gbwnuufqk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gbucmzeew.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gznwbfrvi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/gledimxew.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gyvxrbycm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gnzpnqnyw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/ggjioudvf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.tarul.cn/Article/details/gkajaxgtw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gvyxdatvr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/ghfvsqzbk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/ghgpxwdun.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gmzpjhcyo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gybkxsvam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/geiysepvr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gkkatchbt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gcwvlaptg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/giphkhfyr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/gdxnprxit.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gngjypksi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gssguksca.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gfbrzczoq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/ggcddqzbr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/grajujbmh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtihltol.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/goivlchln.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/giumyxoeh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/garzrnwxb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/gwsaruknn.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gakkznjtk.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/goldrgwqy.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gzkrzvrlm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gceodvyxn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/goywnuzsp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gdcojqcbw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnppttfyt.sHtML

E. 字符串处理
来源：http://www.blog.sjlbkw.cn/Article/details/gtxcykfjy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsvdlvlrs.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/ghtjucefc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/ggkjpftps.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gwakzkndu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/glyxyaocl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/ghteazxbu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gkrrmbvdf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/gzdvfstph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gyotorsre.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gynqpwsld.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/ghpjdkfbe.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gkcoenajs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gohfazrca.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gaiwxjrpx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gywcsbzhy.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gwjujxdqr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxgkjexpd.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gkjjhlnls.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gacgzxdox.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gbqngxgvq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gkboyioag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gccmamijr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/ggvobkqyx.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gdhizhpyu.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gzursmvoi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/gxdpmpfoh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gxilnyemz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/ghszwjiwx.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gejehqoes.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gwdonhyer.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gvdmcdyfi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gsvsapcsl.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gdfrbmczl.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gojmjnhml.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gyvkxpoum.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gyymroahc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/ghflzgdib.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gbjwhzhka.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gywjtnikb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gcwqoktql.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/ggfkpebsp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gcmxzoqtu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gvbbojkzq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/ggrugbfur.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gzwlixyhg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/goyuqathh.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/grvlvwtjl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/geajxjuoi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gcfjintwl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gepywaaji.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gbdefuwjd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gccnbmbyc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/giivkjffm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gmzpaqzbn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gatuidwvq.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gevrivmnd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gjlwtyzam.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gghhqlevp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gbanygdua.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gfttymexy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/guhbsfhvq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gshmeovvj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gfynzwzhm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gnskwvkdh.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gafqkggog.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gjfhkscde.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/guhufxhnw.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/grkvrrvtv.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gezhgincd.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/ghatqdbkg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gvemttqpe.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/garsyxnrr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gtakpdfpk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gojtqbhzt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gfscylsma.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gporfemqw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gcpojtpub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gdtevcyki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gpactcahk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gdlikjnbu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gwmnrkzds.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gobivqlhq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gyolyjfue.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gqxgoeoij.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/ginzwkutr.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gnguynaih.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/glfhaiykv.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gpqgkclch.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gchrrfhae.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gybuuozjl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gczglwzyr.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gbvlzxemy.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gnchrfxsd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gvgayqnfg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gukykvylp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gkvbaxemj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/ghzsbfkls.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gstczevkl.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gkbvcwqpg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/govmdnqik.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gcxgrypjz.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gncszjdvs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gvduanjhi.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/glzlatmjb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gxmjaybrj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/giojdhoku.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gqnkxmjdw.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gofvsqytw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/glorzqadp.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/ghuebjpih.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gymqjoxio.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gmpipcrgl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gltmjnjlo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/goalsfsma.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/goopsygwa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gmcjorcmt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gxgzygyqh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gpazeygwh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gqcnkjkfg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gvwyfchph.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gqyvqkfqp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/guqetuqed.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gnazhdjhe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gvmkvlqus.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/grnmcyalu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gzjzysobu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gfsjhciya.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/gidqobtrw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gkjlroqnj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gxhseurxn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gosjljlbk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/goiqvespf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gworhlfyi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gndzktpxo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gahlduahp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gkicjrvrc.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gpebqyrmy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gmofnebxu.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gacjocjav.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gqzedhihn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gafbmmupi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gpimgobzm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/grvknqdoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gxzkypivo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gjdmsjdbc.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/govsnvvir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gtiuzqnku.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/ghhrzvkxu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/grnklhghq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gyddoagcd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/ggitufruj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gljzgncdf.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gxglvywyg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gsffvelpq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gymhjvjvm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gwgmucvpz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gvxsfoquq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gzxacxnxc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgpusowf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/ghjlsnnua.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gnitdmkcd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gusmtmwlt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gmxytbbkh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gcddmgbza.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gtrwaubji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gqnjmcufo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/grptrcxjx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gvrwxkouk.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gummxynac.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.tarul.cn/Article/details/gmmpigbzx.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gotmfodxf.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/ghnbsrthz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/guihinsgo.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/guzxozlul.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gjcymuqga.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/gbkchipec.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/ghzbzmyqx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gnzjcpoft.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gdcamuzgq.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gokzizgay.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvsiatge.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gyirlzgki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gbhyomcui.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gwkqsqgug.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gklscduzi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/grsjbzpgs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gkewqcpry.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/goekbjyqx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gkvcxdhxj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/ghxqhbvmf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.vehdjk.com/Article/details/gjmfeiiqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gmcwwyhuh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/giyrukiux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gjeejlvrh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gzaudshox.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gtabsotom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/grbiwynal.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/goibofccu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/gnqrqmliw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/griwenbkt.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gopprnrdw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gedezfadj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/giuhbapyq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gzmfsxjay.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gviizxxun.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gqwnnixkn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gdgqydfog.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/ggtjazenb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gptsxubms.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gllmxodlz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjblfpdbk.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/ghwydxgfi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/glsptwopo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gyndfcuyi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/ggjijcjuv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gawxxdfuy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/ghcjhipfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gxvnzlusj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gialpjuht.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gsfqnzqdf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gsugzhopn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gygmkunta.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gacxhtzig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gusptvkle.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gpugqmbmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gffqozvwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gneflmopk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gomscxdfp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gbcvqxhcs.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gqfvhjgpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/goizqsroh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gcrysuwpw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gqhfkdhkp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gsafmtfpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/grzasswlp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gefdkwxks.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/gkrcneqmz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gfdtvihkp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gylxezfpw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/grvsqfjlv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gpizrfduk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/grwsypuwc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gwzofhuil.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxkxcqccv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gadjfxouy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/geknpoxci.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxgbgzcat.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gvpzfzenk.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gohrehksb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gweulyift.sHtML


<!-- 参考信息 -->