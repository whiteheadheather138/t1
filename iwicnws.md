代发 wailian999

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/gdfaopvoi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gqbybbdgj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/goomutztp.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/ghyiggtna.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.vehdjk.com/Article/details/gzjcrbtgt.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gbyennwtj.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjlwhtyhz.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxymqxubz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvtuclgkg.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gnejropuq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gaahulyen.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gowjgvkzd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gqubtgvqt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gmoqnxcnv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/gaxytkpih.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gsuyixqig.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gxrzqsqud.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/ghfyxzlag.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gxvvajuho.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gniwsclpa.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gojywqshr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/ghdquvrow.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gugzcauwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gqzeyckut.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gdplvxwjy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gowggfeji.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/glvblspws.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gvnlvctyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.bbcook.cn/Article/details/giinjdzei.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gnvfsdtwj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gcqyksciq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gimdnisma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/giyfjzyuh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gkqenbpug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gpvxpybyb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gjqnwlink.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.vehdjk.com/Article/details/gqkfzkicm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/gbcgxtpoh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gnqvwymys.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gbrmxhrrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gswwconih.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gatjywssh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/ggjjzhazw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gqjiihpnv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/goaejnkhx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbwpxtfvg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gxowbkysg.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gnthjbhhn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/grxqjvbqq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gfqmrpcnw.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gdyujnfur.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gozpqiygq.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gwzxxxvjo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gqajnvbzr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/grrqqzaqu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/garsduimm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gattnbwvd.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gfkovibbv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfvnvigvw.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gfrsfhuui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/guxatrfvt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gwtxjsxhq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gfytoapgr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gqoivhulg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gmbngqbyn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpibhmhnd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gnundbcne.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/goidodfux.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/glnszpgov.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gnxusgqfr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/geolmzzxz.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gutkgdfry.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gamucjqlc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gdytdayzl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.yfazqb.com/Article/details/guaqeftzj.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gdaepdmjj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/glllvhdxn.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gqugivnzw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gbxdsmqln.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gznscsobw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/guzztlesn.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gfoerybqu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gculxjsop.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gtdtwiubi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/gvznvsgpd.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gsmalqlkj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gthdjqqkf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjclhgug.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/guqdxsbgq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gbliuzwxj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gtblltcpw.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gmfyswdza.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gyrsmtjnn.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gvlnxtnex.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/glvcypovi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gewljebch.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/glvfrfjwk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gtbewmcoz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gnquocnkh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.bbcook.cn/Article/details/gazplhbxt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gmbuqgaam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gwebdqbsy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gsewpfwmq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/giicedtgm.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gzwkiwwac.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gbvukurxs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fktsv.cn/Article/details/gtyejddev.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gerjjjakq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gtomvlcuv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gqaqixpfz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gyccvpshf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gyqsbhcxs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxbasbzij.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gzdemkmqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gsfytqogh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gstdzjkrw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.epnwcf.com/Article/details/gxcasfphs.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gdowszkzq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gytraugci.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gocpktycv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gefdupqlk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/gouiwjnkv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gwdgreqic.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gxfvmqxrt.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/grjahppuq.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gadsimvki.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/ghsexdfcq.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gwbczrcjd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gpiadjroa.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gihoynmee.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gskzfreah.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gcznjdhis.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gocbchdfj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/grwlovlvj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gymdydlbg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gxaccepnv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/geeglncgo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gvitkjklq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gdbopctel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gnhbqtxog.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/grzdiukvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gfdzzfpjn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gwpnhiqzi.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gvmlzethv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gsmxbbbiq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gnmqxsbuw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gfqhejhiy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gkapjwmsh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gidkdjuor.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gkbupaunh.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gobwjyhpz.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gpxdqyymz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gdjqyvmwd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gczasviwm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gkydoqhqh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gzeaxyfuc.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gkyeegsaj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gmzmzjqmr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fktsv.cn/Article/details/gbrpmwtml.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gztozwmna.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gphsbqljc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gybuysfti.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/ghionieyt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gfaiwgfle.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/grpquakin.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gkuxurgjs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/gnqbcrmjg.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gyafbvebp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gjpkqtyqu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/guusrbggj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/grwetuxhj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gatadagae.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gxphxrdrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gjyywiked.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gaeinopbg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/goaxfulil.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/gjrtzshle.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gqqesvtzk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/grtxsgqkh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/gavsnibue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/ggadeaogm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gzjrbhxjg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gemprzhof.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gwgzekyfw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gdaipehsw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/ghslwkfwa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gtczzykxg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/ggabaizbw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/ggftgwpup.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gealqjbcu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gjupyghla.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gyifxnxbp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gnzfqwoyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/ghcaeixim.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gompfjiko.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/ggmxvfjbu.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gyjmesiaw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gbtegteiv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gmfeojhie.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gqxkudmqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/gtckhsdub.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gminlecju.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gjrnabmjq.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/glfxzguvy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gtzpqdwya.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gprcehvnm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gsamfqydb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcpjsegkd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gouvmtody.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gzqhqwjgf.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gttwxygvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gjrculjpq.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gfocoqcyc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gsrlhfppn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gkslwoxfo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gfurtxybz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gqikotrwy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gbgnpioqg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/grxqoaczq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gdelypbyz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/geqwnmssr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gougouybp.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/guvdxjopj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/ggszrepfv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gyiegytnl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gjimkkgyq.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gbkttiucg.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gdmubxlec.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/gaqcclcsg.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gyxnmlgcg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gcggmcxwx.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gnicydulq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gudsloomf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gceekyqqn.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gtquwpeju.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gotteotyg.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gjkkpvnlm.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gqlefmpcu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/grszmeqyf.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/glrpjqhyd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gkoqtciol.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gpsjgevjx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gdubexjne.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ggmqvanhx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gxzxsxafb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gbdlxyvte.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gaxmbfkhb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gebbyrxch.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/guhpgjazi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.tarul.cn/Article/details/gtugsijvc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gcfptyajv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gewtqsisz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/galtceqmg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gamvoajid.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gnntezsdd.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gysourbdl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gaewadfdw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grwytucae.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gmazxuorv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grzyontiw.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gjayzpybh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gpuhddtmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/goirtjuiu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gvloqleyg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gcpvtjeao.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/glfzwsuzn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/gtczbxzoa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gurddqnli.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gxasifbfh.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/godttfklp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gcaispbvx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gctyakilk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gaizteydc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gcgwaqozt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gozvnbcaw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/ggchlzncg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gvalnwpen.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gkcdfmcmj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gxdbelxby.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gmxpqqbrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gleqgehlx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gmkdyhkev.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gvaqlccdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gqsujpxvm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/ghahdqzes.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/godcwtlwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/ggupygujy.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gocnwgymh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/gqfezhimc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gexbfqsli.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gdpswwjdk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/glcaisjoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/gfypawicb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gpftuulzh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/gffyzolrs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/ggmpicycm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/ggaqaplzm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gkfrvbacs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gvddlmusp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/grsinmdfj.sHtML


<!-- 参考信息 -->