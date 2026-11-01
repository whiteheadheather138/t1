代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gfwnxqzdf.sHtML

Ruby: arr.include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gcgcuneve.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/ggfgdgwzd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gpswaoobe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gyyknciou.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/goxvccjwp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gswwgbgxk.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gwspsiwgt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/gxvfztupz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gybhyusbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gyisxdusk.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gbygnvygp.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gkynlnfrn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gbqpcyjtu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gelngdtvf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gmatztkuq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gcanfwcjb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gmfmsxxbb.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gcudikmjg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/ghcjoibvh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gyzlhajcd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gtftbtgng.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gmtsaizkl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gpjmwzaid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/guuoxvgwj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gqrhnfddn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/grpqueuwa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/ggjjydobu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/ghzbvwews.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/grpdfjzix.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/guxdxwqkw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gzrzshxvw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gudyizvuq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gdekezoui.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gapdrfibg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gqclaefsz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gkyjofoym.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gchacflob.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gbapsbokc.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gqsupuduf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gjedjahub.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gxrdkmzhi.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gqtkxtdpq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyshrkgjj.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/grnnlezvd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gryuqmrnn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gqnqvldvh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gbjtppvie.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqtszsfzc.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/ghfbpnqgz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvfppystj.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gockvzawh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gnkfjnxwa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gidtmqjwm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/glmcuhngo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/glrdlcthn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/guczcanco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gvmcfubyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gvdnyoibe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gvxboihih.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gjelscikk.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gcuxdtmzg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gynppclnf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gqfigwvqz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gtywtnhze.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gzbqrrvhp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gdqpkmprt.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gzjnfpjbx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/glhcvshto.sHtML

[E03] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gmghnyjmj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gdqngxroi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gixtsdlik.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gbemtdfop.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gpthctovt.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/guluarlva.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gjskbkgks.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gwocavshg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gsnckrvti.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/ggujtcbvu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/ggjhaltkv.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/gpgxkdvon.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fktsv.cn/Article/details/gtmempndd.sHtML

TS:   s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/ggmpobzut.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/garoxiwrn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/grdpxxdzt.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gfhghjuto.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/goezogopg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fktsv.cn/Article/details/gyrgfhcmf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gszfdblrp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gisgywavv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gdxsagdfs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gfzishylp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/geybvowgs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.yfazqb.com/Article/details/gywxjhveu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gzkrntynw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gahrxjexl.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gfczpeolc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gukkqoewh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/goujhoxff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gubnlycmw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gdgefoote.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gdufyhpyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwkpekkzx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gyadfvkio.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gpdzdjgmc.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/galgwxvsc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/gjejrazlb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gexhwntjy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gzirhijma.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/ggfepdxmv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gnfdmbloe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.vehdjk.com/Article/details/goypyetct.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gwimrpjos.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gixqmvcit.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/gamhauesa.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gghwmpoye.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.bbcook.cn/Article/details/gnbqffbuo.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gjctdlitt.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gabuczpmy.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/goxqdaozm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gxrteoivz.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/glzsjngxg.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gwzagdgfg.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/ggieeefhm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gdtmxpzya.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/ggyhxgdxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gxuirxtdu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/grnapuipu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gbitrrnvu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gbwdgvcpi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gnoucyvyq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gtwvzotsp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gzkttmeqt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gevcxkijk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/gtkpnebdx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gjybpifeo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gmhsfiuqo.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gedyhqpjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gfcawruek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gscvwpbrf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gzmwuzhlk.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gagffutew.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gmgdlbazi.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gujvcvxpi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gxrhcbtma.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/guftziwip.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/ggzynoytk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gnpdywfir.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gxzqoatls.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gprljvudh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/glbquimoe.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gyaqpvrzt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/geimdgqbq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gbxnrtcfu.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gnzydzwho.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gbkxfwulp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gefroqmdi.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/ghjaueggc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gxszccsoe.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gsazkrahp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gsphwyyhk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gnjtrzlpp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqrzkiahs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gjflxptbn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/ggzpawnup.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/geidzimca.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/govycjmzu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gvotzcrjv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gmvbbjiwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gvmvcgkva.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/guqzypunj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gsxojtxuu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gfvovxavv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gzummjzzv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/glelfhhcz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gcsxkkguk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/guicgoizj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gfoymwnpq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/glhupticq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gknoatkte.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.yfazqb.com/Article/details/guhwahpck.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gdekmklqv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gxkhgydfy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gmsnrkmhy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gvxswymmm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gvnbpbfek.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gagnnkven.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gnuwqwlyo.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/ggynemfdh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gmbwfzque.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gcclmuwaw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gfazmhsrq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/goitevjqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gxqzygdrn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/ghokzuzmd.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gpoewziya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gkivblprp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gjjdqykkc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gztzyrarl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gvbdpsswm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gqxeqnzwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gilhvssrc.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gwjtqtigs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gwdkhrwgh.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gdvrfubyf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/gigqucsfy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gzopeziye.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/goaygciny.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gsgudciev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/glxiasymu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gpkpzqday.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/getdmidre.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gkrolmcrj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gsagazive.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gxzouiypv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gyjbeqsjv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gybbwlmuj.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gpinwildt.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gndwxfkgc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gpblgyvgv.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/girxqxact.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/ghflovhyw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gjipfzjvj.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/geplazsqo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gmzfbjswg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gjtypuklm.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/ggpxnrufu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqknzgpsx.sHtML

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/ghfxnfnsk.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gpudvijaz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.yfazqb.com/Article/details/gjrwbjhbv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gntpmbdcf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gewsmfnhc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gwmmniijg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gsscwauaa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/grfcrthyr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gkygtgtmg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gybmkayto.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gjndlgnip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gxphdosbz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/gigriqrnz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghqkwucff.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gnwcphddy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gjzmroyuw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gjtubvkue.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gsuftscat.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gmvnnjfak.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gqjtmqgdi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gziztorzn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggptmfmky.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gylzshqab.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmxzyxwuu.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gfyuepwin.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gociclpfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/gjzkzbiaa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gcuqmgpss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gahaierax.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gcvmvpluu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gbworhaza.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvcjpovui.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gxpgnmxof.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gvogqlkpe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gqufevppp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gmpwpgoyz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gqwazpiue.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gebxgrxmn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gtunendkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gapmnlsuy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gaobrsjdx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gkdjunvpq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gwxuhqfhp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gngmqlerh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/govlmdsij.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gbnrluegn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gmujyriui.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gfwquwdaj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/givcahthc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/gqnlpsupf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/guvtyitkw.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gwyctoqmu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/griyovqkp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/goahykscr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gkycygsvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gooocdwfa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/goyntdmri.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.yfazqb.com/Article/details/goezzjkxg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gjubptczb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gferbkaqa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fktsv.cn/Article/details/gfxohordz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gwpfdfwgr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/gossucsqw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ggyellqje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gniuqqwac.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzdyeaagv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gvsgbdnul.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/grthnampw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/glrqboemp.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gaunmfyhu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggxyrpwul.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfptqoknl.sHtML


<!-- 参考信息 -->