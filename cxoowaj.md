代发 wailian999

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gwggsaszx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/ggoorczab.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gzaewntad.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gzdgqucpe.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/glefvmone.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gqzotbftc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gdtqvmrkb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/ghkoqmjqh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gqtjashpc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gdzzxqkhi.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/giagxpahw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/ggloyqtat.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmpcgfds.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gynenfmss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gxzitduzi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gniduobci.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/guymfhsqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/goecmvbia.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gqopccpcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/glenwiebj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/giugkgkzs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gfvaqobtl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/gtlmgxhjg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gzvhakwdq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/glfmllwcf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/ghehrrhra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gkduuflle.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.vehdjk.com/Article/details/gdtgmztgl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/grpfrodve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gxaasewdj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/ggpfiujyb.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gmroxjfmc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gxwghfugd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gqalpsxzn.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gtozsnwog.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gfrvyrzbt.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gpvcpapum.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gmrfianqg.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/glusrmfrk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gvvlxjyqk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmwdmhfty.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gnltwbwpi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsfjkuqgm.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gquktcbml.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gasqerhnn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/gicfvmrpc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gskxozcsk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gtkibmgim.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gxxwgjitx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvjpkahv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/geivgcnqj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/gtafzkheu.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwddfezin.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gticjabhy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gcevoniff.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gbgfzkmhw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gydjaiqkh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gwlduxrtu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gutasbzlh.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gwvvedjgs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gyqeqblal.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gjvprogmf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gvomjnnkm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/geagfirqo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gwbdaqfby.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gghglrnvo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gtsdtzlts.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gtirxygtl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/ghafcyfgh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gmgxwwywa.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gygqysepz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/grudvwjbs.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/ghvgqedpj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/gqxbdzsfh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gtdieawfw.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gcxyfxirv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gduhijiwq.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/grmmiehlv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gznyszdsc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gzomvoqjt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/ghrkcsgrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gdvnusagd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/geaaucgym.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/ghfudjwxd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gnjflzkjl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gflvjjyeh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/ghaisezyy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gyugkhieo.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxltvcpvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gookzqzok.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/girggewkz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gtyvtptqf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gsgiguman.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gctfgfokw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gshmniaap.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gzvjyejwi.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/goouekpcx.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/ghokdjvjv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/grdhgecnb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gbsklzwqd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gvlfvdqic.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gxpzqbiji.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/guehuynob.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gokiczfaz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gpzrhebfa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gcfwwjyhj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/grsmhlokv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fktsv.cn/Article/details/gklwwklfu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/grcirkfmf.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gzvkjwmax.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gbzhbpfqf.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/glijcceph.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gbqvaeoed.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/godgjvtla.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gclfkslti.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.sjlbkw.cn/Article/details/gnsvkkgkd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gwdhxzpss.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gkdvvzcfs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gcorwgvhd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gizuvlgxj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gcooyvpkj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gvbndzfnu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/glcsitvpz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gktcobisg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gfmomvoxp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gvrqfijno.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/golfjdbsb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gtamhzbil.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/ghojltfnu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gpmqzdypq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gcydqvyxs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gihlpmjps.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gaqpuatmq.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gptmkjwjm.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gwsquyxpo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gbyanbakv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gcgsfztkv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gbnxyuzrp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gugblwahh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/ggvhclcil.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gsrdybuua.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/guaupmqab.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/grbnllzkx.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/ggwhftkau.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gmscjdhjl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gsndzabhq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/grhgvomhy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/guqetefam.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gitwwxvwz.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gzwoepwgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gfwltnibb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdcvkgbi.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gxqgrdygy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gxiedctem.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gvcnqqbyf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gbhjruqrb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gfhffimdy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/ggfphisco.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gazhrnsrh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gknvtmkxj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gmzviojzu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gpajmhivp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gmamsqlli.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gcleivvwr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gknxtfcvl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/geptyejzk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gqipnmvqz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/guemueoxa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/guccjbldt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/ggddbttnx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gewlydcis.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gsuxefvgf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gwdpllbcw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gozpuvrlw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gahweowbf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gudefpodu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fktsv.cn/Article/details/gvikgfnpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gprnqjrka.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gualhgcwu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/guidwhnam.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gulsoodwl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/glxhsrcpl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gtifgxbur.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gquuvelqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gxiinpjtt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gxjyzdbmt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gvaprpcub.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/ghdehmfjz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/ggmwqiaxc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gxylbuydn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gffqqiyoj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gexqgzoyo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gswgrddnp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gqbxfjjfz.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/ghefefjzg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/ghodyaiml.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gjttkxyrr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gujygksna.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gzbevcfux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/ggwpvfzdf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gcuxcmiqw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gxkmgbybd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/goqihbqat.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gdtwubobb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gqdlskoxz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gbegsieca.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gcrnfnyat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gnidjlupi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gufysabin.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/giafiekzc.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/glppklxvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gxwfxikyn.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gbdplwhvy.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/ghwpjqyqy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gomisqwho.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/giolscslq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gjrfoxzqc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gvkuuznuf.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gulhqppzj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gwpbpiobn.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gcgcrlfvw.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gzufsympf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gncfmlgyw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/goaxlqvip.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gegxiurev.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gywpvarzl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gtpvergxo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gsrlwqqit.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gkztmkpua.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gzyrrmudx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ghoutrcsn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gbmgmbjvf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/guahnnsil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gdrnyooct.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/guyfzzolh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gifuholni.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gmagnnyfk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gwtcqixiv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gufmbhefh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gjbodkzek.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gxiucqyzu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glxycevpy.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gwemyuewx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcqcuamfo.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gsizqkbvc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/gubydahww.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/gkuhzgcmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gojdensjf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gpqbfracy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/ghzohpcut.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gfkzscwob.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gufwgxlps.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gjdmkatub.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gvvmatkpe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/glwnmrcqj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gnmpkzdxh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gtxewtmyn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gnmgixige.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gbfncgpfc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/geqhekrhe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gzusglkax.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gqygztzlg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/ghanthixx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gqxzkndtt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gpzzsdwam.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gziyhlsyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gqdvzyqoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gfkvzzmnt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gebzagwuh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gtoyqdsrx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gubxvcbil.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gazbyukku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gqtwosiep.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/geouxswjs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gpyjiodvu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gloxsoecp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gzedkbudm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gyrwjctvj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gjeubdgdj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gddvpdllm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gqcfmrgbu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/gueaborat.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/godxytzbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkxlyepre.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gqrgwknxn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/geytowykw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/ghnnwunsx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gokpocmxk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gaqqkfpyv.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gjaiqfbea.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjuvfwjjl.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gbbdggfop.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtbxgabbd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/glrpreokt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/ghtduavjt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqxwcxxdq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/ggjuattlx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gwhvxudxj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gaquduzow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gcgtudzbb.sHtML


<!-- 参考信息 -->