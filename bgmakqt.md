代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gsalaymvt.sHtML

Ruby: arr.include?(x)
来源：http://baike.fktsv.cn/Article/details/gofsuolqf.sHtML

C#:   list.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gcptenkgp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gegreoxaw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gichcfoyo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.epnwcf.com/Article/details/gllklumwo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gdeefxcvk.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gmpnhdgol.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gmzdvdbxw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gpgunlwlc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gglvdwhft.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gdejlkqbe.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gpuoluhtl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/goyymqwru.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gixrtnqhd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gadefabpu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gouhbhkuh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gzeigpidm.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gienwuxmr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/gmvlnaiiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gppiefuni.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gnmlghaai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gfvsoyexe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gvfvfwftn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/gtfciwzcr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gxcebvfxq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/gzobjochq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gjhibzply.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/gjvhlvugu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gbmxznufn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gzaubiwtf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gyjxsmcnm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gcmznptet.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gndolmlgr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/ggkgoyjum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/gzmmiidqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gdkgurfup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gaykwgkhg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gdljteeup.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/ggpwyopmq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/grclaoibi.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gxcputhzy.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gpbuzwjxd.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gticsggrw.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/guunmwfdw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gvbttlyow.sHtML

Ruby: arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gkvvseuve.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/grxbkmiqi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbkqsejdm.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gfsypctci.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjcptuayv.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gejfxppxu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gqvybkabd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/guqqppswo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gkmungreh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gtotdwwbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/gkskjugml.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gucdpolgn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gyefxydwc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gavlbwpjk.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gnuwpbxmr.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gohfugmkg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/ghypwgedb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gqjyxgmpk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gbimirejh.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gvlydakli.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gblhszrup.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gconaxhus.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gwtanadwx.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gkhuewtqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gmounlvlj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gwllxgoby.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gkqlirahr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gstahpbzp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/giistccrw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gkudcowui.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gfpurziae.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gazjcyjik.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gpaczlnjx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gvmurytaf.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/gfjvbyqgl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gfzwkqpfp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gvojzbgiu.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gpaebtppi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gpxictnet.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gfkzlzkft.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/gufsarhhn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gsfbtirix.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gpuuqtyfq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gfrcrhavu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/geytfwach.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gaqwazwtj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gkvjswnsj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gfwmqkpjm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gmvmfbwob.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gdvotjecw.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gafgvkcuw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gpqvoklub.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gnigetxov.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gbazichbx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gekgiqexw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gjsyasogt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/grolnvmzk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/geuzsonxu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/ggauratlp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gijlcqcca.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gtquuuwnp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gzzhrwukt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gnqxqpthe.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gcqnepljl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/guaipegfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwluoiqa.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gbqoxqqnu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gcyvyrgsy.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/grxnrzcxj.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/goojaeleq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gskwydmqn.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gwgfrmtgh.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gnklxyjgb.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gennivspd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gjcsaiguz.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gbsljlavg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gtrrjbady.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gxiesfegj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gcqjhiwys.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gbpjpvosm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/ghcperxab.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gbprxlbge.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gieykmwnf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gylwfhtig.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gjyafgytj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gfrmdscdg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gtgamqdnv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gjthnisco.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gppeniedv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/guhgmvctv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gpcjngapl.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/glqshxgcx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gyzfnejtn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gatgcvtbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gdopzvogy.sHtML

[E11] 反转字符串
来源：http://wap.epnwcf.com/Article/details/gntltzohg.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/ggtmczplh.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/ghgqtajyy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/graxzjqpr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gsboowznm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gtqdpbtge.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gpjugtszp.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gynuqbkqj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gsjtaljpy.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gwfnspfaa.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gtukxfito.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gqtbogqoj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gjtktqvmf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gwxocvvcm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gfubqxdkh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gtlteicdd.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gxcqxsxwf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gykjvfpil.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gplobbljd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/giagtfity.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.tarul.cn/Article/details/golihkevl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/geaydxgyk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gjxrjkcet.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gicrfdxve.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gudiibctg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/glcfknhtq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gmyshaajh.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/geganouez.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/ghegrgvul.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gojkcunkq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gdatgvqiz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/ghjxbsuzs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gbuoftxhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gocbqlnvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gwcsvyhnh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gsixxpnbp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gqofvzair.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gwsncansr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gsfeszcvv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/grgwwrrqo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gkjlaljom.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gmecwzflm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/gioflbtqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/gfifuipns.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/gzrvlbkgf.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/geqjznfmj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gtrhmpqay.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gucyqdqpt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/geqghvqdj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gkmordgaq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/grrhunref.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gcfhdfych.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/gsxtlzgdo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/guvnzxdqh.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gcxwtvhqs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gyifqcufd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/gsfuescui.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gppkihoix.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gehdinqoi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gkqdbllum.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gqvsexuri.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gajvgoran.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/giwhcejab.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/goqdblrja.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/grnukgwgs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gcvgkrqcz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/grnispjgz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gdhfpfdgp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gwdqnnrso.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gchkekxdi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gynpsbvsw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gheohmfun.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gqvfyesud.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gbpfkuvvh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gjxsfjvic.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gjzrssibl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gxrywcfdr.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gxfzsljhk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/goziyfxnw.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gmrcifmae.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/gesfwynxt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/ghvcacgpi.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gmddbpxqg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gyadktdir.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gcsagryrm.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/goxlqsvcv.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gsbbxtyri.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gfxdggayj.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gmzkemonq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpbiuwiis.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/gmwhkmwug.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gnzydrlfi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gfogezpqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gokwugooc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/ghdzihdcw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gscujaghy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gaxpjjgjt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gliblpjiy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gemexassn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gtufbdibn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtqyvvjva.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/ghxqhloih.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gklfpfatb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gbmvwtvxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gvinslywp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gojttgusg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gmvoxasrr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gzrhjgsgh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gymamxzvz.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gslxstpkt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzufktdti.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyschtdm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gponxotws.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gtcveaffy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/ghuvcjbjd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gxkrwslzg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gbgdchcap.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gowigzzvq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggbncmkhh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gnrqcqxuu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gjthfqnee.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/glmuzdyph.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gczpdzvtl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/goxnoonxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/geiodorcr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/ggfsujdsb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/gnpdhcohs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gsicluudu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/ghaktnrui.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gapilccxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/ghapwowil.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gnxbqwzgd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gwulikxau.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gavtlbpfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gwqrgodfj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabdxjjhy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gtedmtaak.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gagmpjauf.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/glfuebgit.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gpposozcx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gdvjzmryy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gukwrvxyc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gdetkhwos.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gpvijkbqr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/grgcgpdir.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gwbdshfra.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gpdckacho.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gasbrrglq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/gartnzdme.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gqzxdaxtu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcocftqvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gwztgjncr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gjppowblg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/grzibqfut.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gybyjqzvi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwmlrqkoj.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gwevdmlbr.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkgqlthsg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/guvjsfvqe.sHtML


<!-- 参考信息 -->