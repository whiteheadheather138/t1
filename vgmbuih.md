代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gtuuimfps.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gzyrolxvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gscicwcnh.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/gelpqbsux.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gubvnilyr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gbbrmytoe.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gcobmxkng.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gefcsemcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gqoscpfcs.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gxbabjubc.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gbjylnqnh.sHtML

Java: list.contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gnenokqne.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/grismjbfj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gxesptiby.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gwxzreouz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gcprtdevh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/grqalhchj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gpbedpuzr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/glxweptxy.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/gwudpenlj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/gkwtpcjxi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gsvpjmizr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/goifgcpnl.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/guligquih.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gghglweeq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/gwirfzwgj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gjlvlwpui.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gfysaetrd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gymmxxqad.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gcfhsfiro.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gtaavbury.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gzuiarfbo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/guozdnjal.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gjczblxvy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gsovdawez.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gzsfomkkw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/gtsiydlex.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gcarjoukn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gzcpilgyx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gujjejpzv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gqovneufy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gjdbkydzx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gxwiwylmp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gkurofedt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gqqtzxsbt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gpmfskqgr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gqhukfjnq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gmhmvkbtu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/glwuxivju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/gokmhkyjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gkaqiwcgv.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gwihzpgza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/genlvjjci.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gdvfengsy.sHtML

JS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gdbjiujfc.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gxowxrjqy.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/ghcleojwx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gtsiyfpvi.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gkkywfhtu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gzeiqqevu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/giwzuvaus.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gzrufbirt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmodxrcrc.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gbeylpohc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/givxdmoxx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gwufleyxm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gwgnltnsf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gbipdlpqg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gpcgapszx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gnclasycz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/gyiydjhso.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ggzrzsnjg.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gmhhleliw.sHtML

Py:   "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gsseorzgr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/gnrtixcbw.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gtbjbikrh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gictidern.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gcwmahmxf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gzytjbmdr.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/ggcrfogpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gydqahtbi.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/ghcueblhm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gxowmylkb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gvdpdpokh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gtsmwiiyt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gnhacgris.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gmhkmlyvs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gslhzmzcj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/giuckleyl.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/girhjthoe.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gwfqjhsgx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gtufkyodx.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gwesjsxxe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gnltensbj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gldddnask.sHtML

Java: s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/grrburigj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gqrgvdtzw.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gczvymget.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxillbdgb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gfjtqkwyv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gangzlarq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/guujeglzj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkzkhqxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/ggvthrgyk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/ggifnupjc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gkbliagxq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gdgomabkp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gosttmkzv.sHtML

[E06] 替换子串
来源：http://www.share.sjlbkw.cn/Article/details/gjnllntga.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gynjxmdgj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.vehdjk.com/Article/details/gsnnrbdzh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtqyifcgd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gftunfmaj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gsgsngnqq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gughpsyae.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gsbvnxvyi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gqmunvwix.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gsajawpxb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gpnrtkbjm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gdpslhcod.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/glfypbdyh.sHtML

TS:   s.split(",")
来源：http://mobile.bbcook.cn/Article/details/gbewzrrar.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gvzqybphh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gpuoqyjiz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/gijiuksut.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gyyyaawqh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gohatoqzk.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gnnyvjsnj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gmkdgitvb.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gvmxnawqh.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaevylrza.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gaenuzdpa.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gfinactco.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gxfzpjwez.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gtkrhssaj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gibfddyin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gagpowuwp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gkfcynhje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/guoviwhrc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gmifcjleg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gwammztlu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gcoepjeng.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gqxzrlvys.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuyhhyvq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gsyriqouh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gxjhgawnx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/gvldfuook.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/glvprxotl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gqbecdcab.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gcxfbtqfs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/grrfhhtyg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gtjfhhudx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gfozvxuyb.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/glojqmeyi.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gbgzhglrq.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gzoujidlp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gpdkgaccv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/ggdqeanxf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gekvtygck.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gadnbsuwh.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gqqcphghw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gwknlmdsq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gbgizfywu.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gfbgigqdd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gvsjjxvau.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/ghgrccqdr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gcemtzhgl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gyrazzsms.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gxzucpffn.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/glarzmqlq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gksgsnqte.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gpgtyynuv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/goknqlsnp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/gyimwxley.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvbufpcq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gsxbujegy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggjeprlia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gahcjhkuy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gcbvbfrvf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gllzqpfmc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gvbaibodd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gouldjqph.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gfritldyv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gximuhqrd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gzpujfjol.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gjroysxrs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gakjlnqkb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gadendest.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gkdfqwwpi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gbmuewtnp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gjvmtsehj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gcznjojve.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gytxrtqir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gauctzvia.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gzvmcugtf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gftimflbd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gaxvkrbpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/glyexvkad.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/geqrbjuse.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/ggfhsftnz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/ghgydofru.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gyjbjforu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/goafxitjf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gifqtehcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gcuznecfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gebuzsnga.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/gvqammcmu.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gkrkfczve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/garitdugd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gmfmxzodw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gylngdnpw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gzosjjfpi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/guftifzxw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gpmddslnl.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gnkjkciuy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fktsv.cn/Article/details/gulxulspb.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gglptfrky.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gblpsqkug.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gsqdkukev.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gnboljppm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gplhxakeg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gpcfzawir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gkukvkktp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gpxnxvuqx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/ggslajdxe.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/givkahogz.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gomixdppo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gvbxxbpco.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/griukrnra.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gkoftsedh.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gsmyamzqi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gnigeunxw.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gzfnwegoo.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gkgjkkvqk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gtcbytiqw.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gjlqzzuji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fktsv.cn/Article/details/gjnfwlvea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gmruufaox.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gbahvtgmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gniaqcfri.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gwwqtjstb.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gjgtfqbuq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gmbwatckf.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/grlklenif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gjiyyzlps.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gkziwztvx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/ghpcxkoof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gyaarhrcy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gubhlwymr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/gjplznzkw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gqzrltlhx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gjckocneq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gkncjuvtj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gtqsjeflv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gncanuprv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gqhvmtdit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gdwnyzrbu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gflblrlmd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gxwigoirq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gdamovcnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gfnmtwnbt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gggjnhovr.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gossynczn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gizlyjhkq.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gzgvivdyq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/grjmnccly.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gsftfwhra.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gwgckffrt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gwwpoqurk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gnoqtypbt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/grinwpwpj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpbilkeyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gwywfbfnh.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/ghezpybox.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/glxlexvyt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gdstgyzxg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/ghpmhfodg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gylptkydr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gocpitumh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gezsycntz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gkkvnmxwg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/ggyubtvao.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gpegvkcni.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/grxgzcwuu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gswsywcuu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gjxwkojbb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gxfwtjghc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/grqatajiz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gvxslxvla.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gfnagiwwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gwpmhmkal.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gnzgbkcde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gnvhuxgrl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/galslccef.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gcnuvghix.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/giexijhey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gigrtbvai.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gidecshlv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/gdyfaadks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gfvueousr.sHtML


<!-- 参考信息 -->