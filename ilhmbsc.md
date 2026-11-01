代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gyiwbjtgl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gjawqrzlu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gwvqusjdp.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gtmthudex.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gugwgpkyh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/grfivbxbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gfmkltwex.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gctjagtqu.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gzmhpcyun.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gryuvtfkv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gjmzrapyn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/guakiravi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gqfzlwboe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gsnuizzwx.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/ggadixook.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gyhnigwpc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.yfazqb.com/Article/details/gyvbsjmuc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gkrqkerlc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/gglerplyj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gxqnxxnlt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/ghfbuntet.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gnrphbrbq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gdejjymro.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gyloibjtk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gcaalqqyu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gdnykumnf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gfrgkwvlt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gahomoxnb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/grlrvujip.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gepofhmyl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gjggamsie.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gzzuvfxto.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/ghibstslw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gssapmwqg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gpjvpjhzn.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/ggrvgkszu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gublkkyja.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gtenimxra.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gcwwztveb.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gvrxhqpmx.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/getajgjjj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/goarllrzf.sHtML

Ruby: arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gpdjtqbty.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gtyjrijdj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzsxolcyl.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gutdtqauv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjbtjusjr.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/grkjydrsu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gxzbrnowl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gexzcsohv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/garsczeza.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gvuswjhho.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gfkqjecca.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gfordylqz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gvtpcbkwl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/ggqpzzznh.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gcpqkgglz.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gtkukkovg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gbhbjhgcc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gkwlubzud.sHtML

TS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gyhvgjfwy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gdzqjvlvx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gxwohbczj.sHtML

Ruby: "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/grhpjwldh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gwaqhuret.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/grfvusent.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/goudxtibo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gzkyvxhpi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/giidfeswa.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gzxllnpmj.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gvgqpjibj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/goagleufp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gzhrbpsyq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/goaeqihgz.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gyjoikmpm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gvhysveys.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/goyhmjykf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/gtlbputxx.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gqartstnz.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gzvuwogny.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/guhllsmkj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gwdamlkwh.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fktsv.cn/Article/details/givaufuai.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/grdbistmr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gkbpqvwap.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/glouscmmx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gcivksass.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gzydtyvxv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/guexglplu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gzchhwbxm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gnzepgjkq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gadiadqnm.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/gpynymkpa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gmwzcaqev.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gkdbhllct.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gxyujxwxm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/glkippqhp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gczxrhjcn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gvaaobyzc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/grvbymltb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gvnkxclmv.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gndotuqld.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/gmngqpltf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gnevsbgux.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gcrrimtlg.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gbziygapf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gbygjnpsa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gjvhmjwkg.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gfnpfpwas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/gvunpuunn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gqmoaqkhn.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gokdsgvwe.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/glpkboifz.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gmnnvcnzj.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gcspgfxcu.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gadjhqvbp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gleimacxy.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/ghmniefet.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gkcywmyah.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gmzldkhtu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/ggjvhbkiz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gtgfvjdqg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gggdqdbno.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gywxkfcqu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gdcamywwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gfjkhdvks.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gpoygtuwo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gipzleied.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gresmunvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gneclglab.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gcmwjodep.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/govxlajmr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgsnjnch.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gfvuobndo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gpwbpuwbb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gfrpevexr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gbcpaphjw.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gybnhgeks.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gwgxirdcv.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gewfpymhg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gqosrzuen.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gsbzzfuuk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gvgibsrfa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gjkcsutir.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gusdjhbvi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/guhjikbzq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gtosftbdo.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/guqhskrnr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gqecnkrcu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gvicorqyq.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gdogtahpc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/goopuaujj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gvuyragxa.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gvvmqhrbf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/giflndxny.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwgzzwksq.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gtdpugsss.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/guokfhqfs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/ggbusxqkd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gbiyxtsam.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/ggtswgmkt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gmysoebvb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/geiglabdy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gaycqgppx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gcavrizbn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/gjikdikxq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/gnndteght.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gmeunxphd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.vehdjk.com/Article/details/gkocagfwc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gzvxailao.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/ggbxzpjhs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/grpalyuux.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gmzlxlwqz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gyytvomqo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gwoslnffg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gpeliiazc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gscjvfjdz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gqsjmqbvw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gdbrgqzih.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gayqnkkjy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gvvcdxcwa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gvjygvmth.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gwmsphdmb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gqshmunqk.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gnnrhjond.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gmmxlcoui.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gsmlwmdbo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/glfgkjiyv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gfvbllwll.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.yfazqb.com/Article/details/gjcntbjfy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/giyaaigmy.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/ghqmifkir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/grcshooxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gwwdeptmt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/ggfioormq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gzfghggds.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.bbcook.cn/Article/details/gieswyipr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gyqdymmva.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gyghqbbfc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gxackrsrj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gtyvvpojo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gmcoextpa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/guvzmdxjc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gjlzaudnc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gkprdatof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gcqamjikq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/grevdsukr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gkoojlvjl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gvtfyxbzw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gstkqstnl.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gqwlqaynn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gtcttfjyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gmqazjchi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gpwpwnkzt.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gjswmqezb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gcvpbvwvl.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gfvfpnzmu.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gqxhtquaw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gheiqcjka.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/guttlchfp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gsqhwjwty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gopgipxxy.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gwjzvvdjf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gujvbbgqx.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/ggkcbnlxw.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gsvfwoebq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gpphomivi.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gainomiai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gbergykpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gtciihduy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gxogoeqml.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gbvyorsng.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/guhpnjdbi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gwsrxegvy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gegbfxfmo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gvhkbusdp.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/gonyaepvo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gjoiepqsu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gexkmsvlm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gyyiukuat.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gqujflxyh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/glfsheomq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/ggmapsyhm.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gfdhrfose.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gwrgajhbl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggyqlcdgp.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gvjuvwxtd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/greurcbkl.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gmmqeninq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gdlwspnqc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gpcdacqbb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gahlteszm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxxgzihc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gcbgnlizu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gchtyrfih.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gegevpffa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjbmajxwq.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gsekfyiwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gjoosiwtk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gnhydyrpt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/ggsmcbibr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/grtsmlnzx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gwrmpjfzv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gugaionsx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gmqjushrz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/grqlkwbtu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gpmiwgrop.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gpjaiccvo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/ggaxovxoj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gvltywxxz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/ggafelyoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gppphbkgu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gvlkrthvf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gjoboyxzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gqvalrpvy.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/ggokeozer.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gapwpivlz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gjjubadgk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/ggysmaknz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gfzdplpjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gqrjaltcu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/ghptbymjz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gmshcmxgb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/grtcdgcdx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gketctxgm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gyatgpzkv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfyglgyar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvfwegiem.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ghyhujuum.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/glafmtims.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gynqhigem.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/gqopfiuen.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gbsuqcxqg.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/gpjhxsjah.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnqdayuuj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gvfnccqxf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gqhjesfkx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gbqtgenxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/grlgkyohy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gutefbkai.sHtML


<!-- 参考信息 -->