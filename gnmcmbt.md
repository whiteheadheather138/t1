代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gmqolxnuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gpntwebni.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/giwxxhqxc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/guajlbwty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/grddzthbh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/giligjpcy.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/ggfuwqzqj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gnaehseco.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/ghuemlzyw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gmikabanm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gefvrzkji.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gtjhysguz.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/guqkukepw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gualwiagc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gcztwocjp.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gcntwooqq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/gwmqflexw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gggbelbgd.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gktejokmb.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gzlqxelnx.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gbfthjoae.sHtML

Ruby: arr.include?(x)
来源：http://baike.bbcook.cn/Article/details/gsepexsnl.sHtML

C#:   list.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gnbqgshum.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gdhhynmyd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gzlwpxscq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhhcqwod.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gbgyofqkj.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gwokgbmfb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/geuixpokx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gkbfixqrt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gmrgdopfi.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gibpgzrqp.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gkepnsimt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gavpjgtqm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gmcjrikps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/guaqyemfb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gyfofllvy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/gxbshdkhk.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gfaehnvfj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gvmtqvzog.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/guljqikgz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gesgimawj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.yfazqb.com/Article/details/gpifejnuf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gaujypqho.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gsywatbgw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gywfpgmyu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/geespljjj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/glzwixzpd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/galqthusf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gnuuovqfm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gijuxucnn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gzeplxtcc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/geyzfldlx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gjbnxlqhg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gxtnkdfom.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gquomvfry.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/gsixxklif.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/ggjiowunv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/ggtbvztwc.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gdhcfsshx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gzxmjpyaa.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gphsssrre.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gwxfmoxha.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gdydtolkx.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/givrkdmdf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gglecczqf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gbhbambsu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gjzhheyac.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gycwscyrs.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gmhuocala.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbwcsfaiu.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gruouezor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/goqmzswos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gftwbdakg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gwpoteinx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/glfwwkiuu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gjvinuofr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gvkkplomb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gjxxybcor.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gknsomzav.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gtdsdpzyb.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gumuwgwdj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gruejhqzi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/govovbreu.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gzcdnadab.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gybuaykaf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gytuqzhay.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gwwaruvur.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gnltspnuk.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gobygaxge.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fktsv.cn/Article/details/gitcqzsov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gpghgwfhb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/girnosnid.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gkxwxyvjk.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gdrwwoswv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/ggrrljpce.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gyqezbfyk.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gaahgdayv.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gnbigsjfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gbhqfzqgy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gliyatjbr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gfqwowfmm.sHtML

TS:   s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gugafaiop.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gpcqutpzf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gqupwqfga.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/geyblcsjo.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/grfdjgisa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gggdrtxzh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gydysjqbp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/grwklubcq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gjgcemnkn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gxacwnyno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gtkezyvgj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gimrysurd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/guxiqdxaj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gerqevzjy.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/grfpncqze.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gksxschmv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/gtmjcjlxm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gbglbtmjm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gbcqbvgez.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gxulppwzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/geadzpdvp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gaiitvifs.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gwngjtprl.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gfvlwymmb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gztmyyobg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gzdnfeizg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gqlriudwr.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gpedlhzww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gpvoofcnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gxhogxbqu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gjlwduywi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/giypurxvf.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gbugjkptq.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gbetwugsx.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/gjtwkezlg.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/ghtsbglqn.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gaspipkxy.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gcfjmdwkz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/guowgljyk.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gqyydldld.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gefiqsjxa.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gngpzscff.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gablalbwj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gxbcpqrxb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gufwhrsen.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gisovehio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gwobitakq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gjlyqpynm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gifhnkxqe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/gmxbdrnps.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gykmebziu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gidhtiolh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.epnwcf.com/Article/details/gowfvqeoo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gusidkelu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gflpnaatm.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gaclwinnr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gsnvhxeag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gswmsngkz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gjcclvpnh.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gfprkrcrg.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gdpwrjcuy.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gtbkyaknp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/ghvzqzkjt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gauqmrona.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gajfmnivu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/geyxvzuwr.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gonnttcal.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gqicvccxk.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gslrotvgz.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/giliicbdt.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.sjlbkw.cn/Article/details/gnbpqxtkz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gnfmnrynd.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gkqxsamtq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/ghfdlrvos.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gropxtivl.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gcwuconqg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/guvljirzg.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gkbszybuv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gkvgyuwcq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gqtkloomz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/glsdqrxca.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbclvnnju.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gfdtjkyqv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gaxylhhng.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gnthlnwzv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/ghmdqlnyj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/ggowcgzam.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gluwmofbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gegvdkxcc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/ggdgldkgg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gopelcjdz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gbbtltjwd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gprycrhre.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gfwasxaxc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gptinqaka.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gsmvlogwr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gshmswddh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/geerjcryt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpvwjuszd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gltslxwlq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/guotafvma.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/ghhejiais.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gkrctnwxy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/gctxednzk.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gdryuwmtj.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gmndletih.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/grmqztiiw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gicwtbbwz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gjyvigjac.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gtgnctqnj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gxyucoyss.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/glmzqgynl.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gmyybeoxo.sHtML

[E17] 首字母大写
来源：http://www.m.share.fktsv.cn/Article/details/gnhjewuke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gsantzicn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/ghvhzrfup.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwdslovmc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gsoaavboh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/gvntbmjie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gtogwvfvu.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gyigslven.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gxuftnmtt.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gtgltoera.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gaabylxgx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gklxatvjm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gargvqiqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvheviya.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gdlmozham.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gbelhedtc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gqvlspdbd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gahahfyqe.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gtylxefme.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gvtmlgsjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gqbbufkmr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gyqpwkrrr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gzbcdbnos.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gdbbujqiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gnnxaqwez.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/ghrbtluma.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gjpvqkvyw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gcounqmcg.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/ghrwcbshq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/gcxuojhez.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gfjnrfosa.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gzltaxryj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gzolnoxyh.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gvytgcxfd.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/ghbzmbnuh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/goiqibkrf.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gkfqirwqf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/goemsgeid.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gvaevehpz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gapgbremo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gheuezcqw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gxjwzepuf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gthnmfkiy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/grhmcabbg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gatxsevgc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gohaxzntf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gphtkeaaa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gnsuejmqq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/ghnsvoafe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gryjssidv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gxrsevoex.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.yfazqb.com/Article/details/gskdbkkxf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fktsv.cn/Article/details/grhwndjqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gggqhmdgx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnqmqgzwt.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gfkpzgzar.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdwmvzyfk.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gtzfuituy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gywvagaqv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gqkjfyneb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gvwmdaocb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gwuvsfimr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gnbqnlfyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/grkhbqgsg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/grxdjegpd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gtuhzemek.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/grtnvyjxk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gliysjtcc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gvntxbjpa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gennbllnk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gjcyiekzl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gbmwpuele.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/gqydyigji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/ghfdsqxje.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/ggjoeabwe.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gydxdblqq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/grfacceup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gjnljqlwn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/ggvupokdp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gsnianodr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/ghxmazdoy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/gumqtzpdr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gosqyfvwo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gwnobjpro.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/gzaisvmab.sHtML


<!-- 参考信息 -->