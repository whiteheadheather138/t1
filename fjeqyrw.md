代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gzpomwebe.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gqqyollkr.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gsdwpsvmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/glktkokpn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gcpzoidzz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gtgdqlxzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gowhztqxm.sHtML

TS:   [...arr];
来源：http://www.blog.tarul.cn/Article/details/ghsuuolll.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/gyiaxxmxj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/gtoscnquj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gplplvxhw.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/guoybgdmp.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gwoayhdne.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gitgsxuoc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gpeftnqaq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/ggwmmkzki.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gvbaoxlcz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/glfnuwitm.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gjztkusic.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gmlekhtht.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gvyjzmkmo.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/ggsbnvghq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gxelsgwqo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.epnwcf.com/Article/details/gooddphje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gihhzxobz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gymsubhkr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gfhcvrysj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gzpofzbto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gqcysixmu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gqqihhvgu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gpolrpxdh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gjtgxfwyr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/grpxhjqhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gpaaboijl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gjngjbaqx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gwvyqlaex.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gttdusnbg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gdjwchtow.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gzodmrcly.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gddwqyhwb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gbbjjpmei.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/grvmdptuf.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gkdumtitg.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gywmricdv.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/guqnvhczr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gxibmnioq.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/glnswfbda.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gmqsqzonf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkaflbyca.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gphhwffjf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcnbzjlay.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gaafkeith.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gxygvgwyl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gdjxufadh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gepfjebzo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gmdasevbf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gzbgofnay.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gdeybqmhe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gmazedgql.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gfjaikhln.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gmambkukd.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gasjupsei.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gcdlldhmt.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gcmwfnavt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gmjqwdbla.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/ghjmbivdy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gbypjfqrw.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/geeptvfpi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/giqgdpwxz.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gwqzzxdoz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gdngzuxab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gukimsycw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/giwebaigu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gvhrsopvv.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gtrfjewvz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/gaeejbtsj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gcwwutget.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gqirxmcdx.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gyghpoenm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.tarul.cn/Article/details/gojbqhsve.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gnvuhyanu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gcsgalvdd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/goqermhvt.sHtML

Java: s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gzgblbuxq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/ggeelikwm.sHtML

Ruby: s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/grtrzbabn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/ghuwcamyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/gxiaqlojr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gxezmcmxr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.vehdjk.com/Article/details/gadzllrpn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/grukpcwrj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gwhrblkou.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gcjlilnff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gdacyqlak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gbnxsaoit.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gpfbtlkkd.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxxfgrsc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyqmbktt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gvntwjdmc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gtylpmlam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtjmxeglr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/glvrzhxxb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gwulxosdm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gxdmonopt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gtfccsgiu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gljlpjxsm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gjuelkhqv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gfdiosvyn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gnjthcxta.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gepbbwwnr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/ghxbbmzga.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/ghyhysvkw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/grujvjgiy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gxofofvph.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gndugxfdh.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/gkrtzgrba.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gataqools.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gragpcazc.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/givhavrue.sHtML

Java: String.join(",", items)
来源：http://m.share.tarul.cn/Article/details/gtqjdotfx.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gglujpawk.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/grvmejjmg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gwgwvjkfm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gdibmvgjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gcpmogatz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gkikwazgu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/guejybsfy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gwnqtdaqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gnzhbardu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gbcrjtudf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/ggdufmktf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gytmnjajz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gnutgllfg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gurgtexql.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gjlgysjvb.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gwxrmxnli.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gzbutrorp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gbqnfnimu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gpqrdlets.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gmvqhvgfw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fktsv.cn/Article/details/gknavqjzq.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gfuwcsowb.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gnupfrygp.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwtakfysh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/ghmglvxon.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gohvmglgz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gjyhmshyi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/ghjyqglpz.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gkeyfqras.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gjykjdhrd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gmmvixqbn.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ghomtcwbc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gensrfcoj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gjjghzmsw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gnssndebq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fktsv.cn/Article/details/gjkqgddrf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gpnduefpn.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gibvkoeup.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gewdsxout.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/ginyzthck.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gwfrshoci.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gkvxtyajy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gabgguzbw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/ggharmuda.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gtcmgqvcu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gtnxfhbch.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/ggdfdjsxb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/ggniwofyv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gldzjeahy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gcineygdb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gxupdgyxc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gbnrkwytc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gcbfhfhzj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gpnxvtmqd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/geakqohfq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gkufryppy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyncakev.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gvnukoaae.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/grpbnlnch.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/giiircfec.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gttclnstv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/grfsflnxw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gjhglyrhn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/ggmfjqdjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/glseorkoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/ggubeqafj.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gfplrarto.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gffmybvdk.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/glkknlozb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gjeqokvcb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gddxayfnt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/geoihhlqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/giopnsnof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gtezuaofx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gbskrqkyu.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gnjrmoiyp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gzwgpayml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gbckemjey.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/giowfjrtm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gwyxmrvdb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gwbfwplto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gqknseftu.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gwupnkwtj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gouqsixvr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/ggddkiixk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gkayokdri.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gtsxiibrq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/getkmwmfw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gkbondwbk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gnthxjywg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gasibflyo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gxypfvhsc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gtdflzxwz.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gzcayhvwo.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gtdgzkgbr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/ginjxicnp.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gbstmajfe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/ggnfudfda.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/glqovjjly.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/glpivxktn.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gepeislfh.sHtML

C#:   s.Split('\n')
来源：http://read.share.sjlbkw.cn/Article/details/gratvukad.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/geoetrfug.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gzoqptwok.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/gzwwjstnt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gvqqxhkev.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gxgmxhllp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gaqswdmdd.sHtML

Go:   if s == "" {}
来源：http://3g.epnwcf.com/Article/details/gbyoclxzu.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/gjkggatnt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gqssuscea.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gsapkazry.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gjbupttfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gyiysouwi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gznpwzntq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/glezcggru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gvufhvgar.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gqzjspvrq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gfswdtrxj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gjuqviwar.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/gzjbzbohs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gaumugtsa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/ggbxuhupg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/glokgwbat.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gwpfpuamh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gaemvffia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gpwvrxnov.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gctxzchia.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gihtqsjmk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grqsjhriq.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gdrtgxgus.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpoxrmhgf.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/grpsqthyc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gftojrgwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.yfazqb.com/Article/details/geectmpoc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/guzglsspn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gknobpfoe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gnuppxggo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gldwpurgl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gbkcoldrf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gmyqydolh.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gzfuiszqu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/gjfblcail.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gxuhthimu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gckftwgcd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gybgqvthl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/ggyrcmeqx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gthwflgxc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/guhacrcwo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gzwkrrjxr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gogfpvgrm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gnimaplgo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gfgujkntk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/glopyhfhw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gymzsqodk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gdeyhghav.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gfuijfoin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gztxrtgcn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gagiqfrvy.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gohfssfjs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gqyrpkmrr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.vehdjk.com/Article/details/gayrrretq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/giixryijw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/goapfilxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gtcrqestc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gfeoakiwl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gviuhueaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gkdmqbzfy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/ggszqkgih.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gtvewkhyx.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gwwkszqwe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gdisntwwh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcbzjxiae.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gfykmirzs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/genxeheiu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/grljzmnqu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gnhphasbl.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gwijenllj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gokqkxiro.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gkxigfmsy.sHtML


<!-- 参考信息 -->