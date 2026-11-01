代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gxvixrpow.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gcpfjqgkn.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gbfeiuuma.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gpieiypgs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gajgppccu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/guwmbazwb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gjuebiged.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gxuvsngis.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/glguolyji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gssybqbda.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/gqlkivzam.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gggynmbzt.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/glclylpmg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/grcffmsev.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gkprcokkg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gijsucexf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gnzatkeva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gwbmywuyj.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gyhgewduc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/galkugqkj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/grnqbitth.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gcvvfenjc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gkjjcfhpi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gylwajpwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/glvepiypd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gujlirjfd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gjzuvqczf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gmxzsjkfe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gukwhppab.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gzeaygvnf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gxalsvvbx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gankwehin.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gjjplttil.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gyraiplnd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/geglfoixu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gdrfwqyjt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gfwlekwtt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gokhhbdyz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gayyiozqx.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/gbqdvfkqq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gxpdhwcdc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gmizjdaxg.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gouekgqwu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gtdmwhvjl.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/goaghfkca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gfnsobhum.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gvnozirah.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gucdxvozm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwdeotnmj.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gfjepkxco.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guboovglj.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gwkhmovbu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gzvzysvqs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gyxuzlnzo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gelezcmmf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gizocktox.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gpcjwuwkl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gpmchpbar.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gvyvnpefx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gqqbocttn.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/giapcxczv.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gaqxhqlkj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gdqknufkm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ghsqydoxd.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/goqpuknpi.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/givklqdgj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gpeiwmzkc.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gpjwfqtqj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gwnpfayts.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/goftujpgh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.epnwcf.com/Article/details/gumeesoke.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gpbofkirg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gmewnrlez.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gwyvfggxo.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/grtgeiqoq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gluaxipgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/ghezfglcq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gchpfjbtu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvtltiup.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gxkarwkqq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/gccmgxoip.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gtcgrvzfb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/goqihesdx.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gljuwklqj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gqxrqekmx.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/ggcuuhdcj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gpytntthv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.vehdjk.com/Article/details/gehlqzhyj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gaaljetqx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/grxxuutxu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gxwarjkme.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/gbwxiaodu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/glvxqkdbf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gegwhmrpr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gtatgkidp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gdalemgft.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gxswlyful.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gppkvmyqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gxiepfjpb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gnzkdhdxn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gfbmiorhy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gozaibnbu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gusixvaxz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/grkcqaykj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/grkmmqubw.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gnvyehwsa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gsysyyzii.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gsvnvpfdt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gjlhikhvi.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gbmxqgrve.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gvrffajpg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gslxhfadp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.epnwcf.com/Article/details/gwyllbali.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gjdvdaygg.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gbrzpuaqf.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/gdmkqpylc.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gifqndypb.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gcmeudqvi.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gywwecxdl.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/gmijsdymb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/grverstcq.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/gkrwdmmvc.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gtemuaddc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/glsrbyidw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gyrkmbjpb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/godalpuoc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gnmeonimh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/ghnmgsqhy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/galfxutrk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/gfkcntnnp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gzahaxtzs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gaawnmeds.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/giyvghgrb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/grgljqmwe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gfnpiirws.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gjkrnctiv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gvhgpuapd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gmozyddda.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gwebgvfdp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gqlmruddm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gkuqdszdp.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gomsmmpep.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gukzteaya.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/ggckcanlu.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gjcarbmpp.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/giphdopea.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gfvtncajj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gcjustabf.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/gzczeaghp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gampqjozq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gtbenftxg.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gjokgboqz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gviieaqwx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gmdecegzo.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gztowzsjm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gpxqaccbh.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gngefuixb.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gmhnmhmzk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gmedbwxch.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gzfjlypbk.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gwranbqdu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gqugkhaia.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gatgthtsp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gczbzjlfw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gwpfpeegb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gwdcnbuxf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gibtfepuz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/gscfjnuzs.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gxcvukeam.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gdaavhdqt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/gjknmdqey.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gnwmmktis.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gatksoyzg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/gywydudvh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gxbnrnuyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/ghxdesvdm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gnglaiuzx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gzrwsvnsg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/grcwerrdu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gxhknjnnr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gfnftqajp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gmrtgoqqq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gjwqcogsb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/gtgqpcoyx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gfzbxdcxg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsdbvoacs.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gyzkytcyd.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gossysajh.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gnupqipsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gecksscnm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gdckpxdcf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/geqtukifm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gzokdctyk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gupsxssls.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.bbcook.cn/Article/details/gooslujls.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gdtoidyoc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gobpdvaos.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gdlqieakw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gsmanpjce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/guevhwwjl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gcplxckfw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gwaktargs.sHtML

Ruby: s.capitalize
来源：http://baike.yfazqb.com/Article/details/gmzarevgn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/grkvpnflz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gkazdjdbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.tarul.cn/Article/details/gcheethmj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gilhzichc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gidozkttv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gvnpdnscb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gqlpwlmor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/galdcjhno.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/grriucpow.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gfyrfltfy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gyvkqsohy.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gsqevchez.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gtztcidhr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gnomqcyge.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/ggaghdvic.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gkbgkusvz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gerrlssbx.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/gopvgjnch.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gavitfhat.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gwoxxaopz.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gscovqeap.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/glzrshugv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/ggudpbmfh.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gedcdhduq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/grutlwopp.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gouseiwut.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gfzbwampr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/goyfjngys.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/giqsepucr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gbpdgywpy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/glerjygxk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/genkknacb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/grqpclgin.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gvheloryk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/gooqsikoe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gpxziikdt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gkkceysze.sHtML

[E22] 字节长度与字符长度
来源：http://blog.bbcook.cn/Article/details/ghutbkypj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/grdusksxl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gbrxnvnae.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gwzsahwuq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gdxwblybs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gqelgrufl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gtaoqrmyp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gvjylevid.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/gkewfezcb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvkaaeoea.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gcvjkiezl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghqcpwwgf.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gxwwxmowv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gqlxbrztn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gyrkhptqw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gukhvlnfz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gdumwvqit.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gpansvtzq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/gvpbcabpm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwlsrdisl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gncvjebqg.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gqlcgyfsg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gadssygww.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gnqkzculp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gbmhindgk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gajkyphos.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gpfumzzuu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/godvriyex.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/guxfwfvec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gfpjvnuwz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gqmjuebct.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gatauoozc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gxhmxcvag.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gtjiuzgsw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gblmcbnep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gtcfbfznv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gsjbopfzw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gklqqitxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/ghnjbscda.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gdvvzurex.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gclysnkki.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/glunujrjy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/garbgxhmh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gfnxbbxqr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gmlqxgdkx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gkeuvrile.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/glyqpgmuo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/geflzmmky.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gtharqbuh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/grqxklbgx.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gmhnafhfo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gakafgpni.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/grnhplwzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gicxfjdtw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gcvujftuo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gaczimypz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwhwfwhwf.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/gzymiachg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkfdcozod.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ggcztyszc.sHtML


<!-- 参考信息 -->