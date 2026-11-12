代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xvt.pycfn.com

PHP:  array_merge(...$nested);
来源：http://yzu.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://soh.chenjidiqi.icu

TS:   nested.flat();
来源：http://uuw.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lxi.havefunace.top

Go:   // 手写双层循环
来源：http://qxc.xziqi.cn

Ruby: nested.flatten
来源：http://osh.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://evw.fzhhl.top

[D19] 按字段分组
来源：http://wwx.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mst.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://keh.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oav.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nng.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qzz.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://lod.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zlr.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sep.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://uva.zhixingplan.top

Py:   Counter(arr)
来源：http://ypn.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://inv.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oev.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxk.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nih.hammf.cn

Go:   // 手写 map[T]int
来源：http://jvc.yangfankeji.com

Ruby: arr.tally
来源：http://jna.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ztt.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://agd.shanyushiyangkeji.top

Py:   x in arr
来源：http://mkp.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://dnb.xylfe.cn

JS:   arr.includes(x)
来源：http://gwr.yj202588.top

TS:   arr.includes(x)
来源：http://uyo.ppjwa.cn

Java: list.contains(x)
来源：http://uak.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://key.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://pmq.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://umt.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://vtw.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hme.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://igb.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lmd.ybcxt.top

TS:   [...arr];
来源：http://lmc.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://xgg.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://rap.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://lvd.uphjek.com

C#:   new List<int>(list);
来源：http://fcl.yj202588.top

[D23] reduce 累积计算
来源：http://dvb.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqb.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uwn.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://man.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tup.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cyo.jiagoushi.top

Go:   // 手写循环
来源：http://cui.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vem.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xog.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://kny.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qwq.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://orc.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tei.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zek.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rqt.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qyb.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eja.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvp.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://clk.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fql.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nxy.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gib.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ods.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uhd.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yjg.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rkd.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uwo.snrcjt.cn

[D26] 数组转字符串
来源：http://qdj.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://rae.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://dun.ydzc1.top

JS:   arr.join(", ")
来源：http://kqd.sjlbkw.cn

TS:   arr.join(", ")
来源：http://hru.nwbrower.top

Java: String.join(", ", list)
来源：http://jui.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://uzo.epnwcf.com

Ruby: arr.join(", ")
来源：http://sad.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://uoi.tianlin.xyz

================================================================================
来源：http://pyy.nanxuanxn.top

E. 字符串处理
来源：http://llq.jqgufenzy.top

================================================================================
来源：http://nbv.yongpay.top

[E01] 拼接字符串
来源：http://rsv.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qfb.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cfe.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yjh.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zif.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nzx.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ujr.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jdr.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xrh.xuetiantiany.cn

[E02] 重复字符串
来源：http://scr.cdnleiting.top

Py:   "ab" * 3
来源：http://ynn.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://ozv.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://ykr.fzhhl.top

TS:   "ab".repeat(3)
来源：http://nsr.bbcook.cn

Java: "ab".repeat(3)
来源：http://fea.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://fgd.yj202588.top

Ruby: "ab" * 3
来源：http://idx.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://twx.ivvv.top

[E03] 截取子串
来源：http://vzi.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cjz.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ohq.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hux.hammf.cn

TS:   s.slice(1, 4)
来源：http://obb.shzxlz.cn

Java: s.substring(1, 4)
来源：http://iwe.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lgn.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://fcd.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://sue.pengpengdd.cyou

[E04] 查找子串位置
来源：http://dhn.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://jma.bbcook.cn

PHP:  strpos($s, "x");
来源：http://uxc.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rbi.sweek.top

TS:   s.indexOf("x")
来源：http://mkf.zycfv.cn

Java: s.indexOf("x")
来源：http://myp.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://fnm.zycfv.cn

Ruby: s.index("x")
来源：http://mrr.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://cnf.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sen.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwe.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://whw.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pwf.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qwq.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://thd.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bfj.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xlr.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jpu.aibaodan.cn

[E06] 替换子串
来源：http://xwb.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yfb.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://rqj.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjj.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://veo.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vge.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nub.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jke.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://hgu.yonumen.top

[E07] 按分隔符拆分
来源：http://bgr.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lqr.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lyd.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gvl.haohaochexian.top

TS:   s.split(",")
来源：http://lxg.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://ssl.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://alj.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://hxa.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ghs.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://wxs.zhiwuduotai.top

Py:   ",".join(items)
来源：http://bec.hnqzz.top

PHP:  implode(",", $items);
来源：http://udz.pengpengdd.cyou

JS:   items.join(",")
来源：http://lri.haohaochexian.top

TS:   items.join(",")
来源：http://pai.fktsv.cn

Java: String.join(",", items)
来源：http://msv.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://loz.sweek.top

Ruby: items.join(",")
来源：http://oft.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://krb.shuidangran.top

[E09] 去除所有空白字符
来源：http://rmf.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lga.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ssb.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://nnm.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ebb.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://fjk.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfh.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qro.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qre.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://hxg.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dat.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dml.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://jmb.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://tzq.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://cmj.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://umd.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jok.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bov.316326.xyz

[E11] 反转字符串
来源：http://kgj.zhixingplan.top

Py:   s[::-1]
来源：http://dit.jinqigfzy.top

PHP:  strrev($s);
来源：http://ohu.cheryme.top

JS:   [...s].reverse().join("")
来源：http://tul.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://xel.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vdt.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lbl.yfazqb.com

Ruby: s.reverse
来源：http://keu.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://abc.xuanzx.com

[E12] 统计某字符出现次数
来源：http://mpa.jiagoushi.top

Py:   s.count("a")
来源：http://flr.tarul.cn

PHP:  substr_count($s, "a");
来源：http://qwf.yj20258888.top

JS:   s.split("a").length - 1
来源：http://yef.vehdjk.com

TS:   s.split("a").length - 1
来源：http://wxc.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xhy.pycfn.com

Go:   strings.Count(s, "a")
来源：http://elj.ydzc1.top

Ruby: s.count("a")
来源：http://nyl.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://yoo.jyoumei.cn

[E13] 逐字符遍历
来源：http://mre.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://wzy.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rwj.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pzb.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ckr.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bih.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://haq.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pep.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yrc.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://zyn.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://shh.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hby.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yxd.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ups.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wms.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rgp.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vcy.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kmz.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://tcv.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bou.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jpb.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ysf.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://myz.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gkk.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yty.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lks.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rab.hongshengwenyu.top

[E16] 数字千分位
来源：http://zay.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://bxg.jyoumei.cn

PHP:  number_format(1234567);
来源：http://iyr.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jhe.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mer.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jiu.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ade.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://izi.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://sca.cashguo.top

[E17] 首字母大写
来源：http://njw.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dbb.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://urj.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xwf.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jfv.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://atp.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mmy.zycfv.cn

Ruby: s.capitalize
来源：http://uln.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jkt.nanxinkj.top

[E18] 模板占位符替换
来源：http://eft.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ldr.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tem.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sxu.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jun.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pbn.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fip.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iui.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jxd.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://kcn.yuxming.cn

Py:   s.splitlines()
来源：http://xvs.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iaj.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://mzr.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://qav.vehdjk.com

Java: s.lines().toList()
来源：http://fbg.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ymk.dashuyun.cn

Ruby: s.lines
来源：http://xwj.xylfe.cn

C#:   s.Split('\n')
来源：http://cmp.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://hni.ydjk.org.cn

Py:   if not s:
来源：http://lzn.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sdu.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iez.snrcjt.cn

TS:   if (s === "") {}
来源：http://hxv.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://yiq.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://tic.yfazqb.com

Ruby: if s.empty?
来源：http://rnd.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kdr.hfpthk.cn

[E21] 超长截断加省略号
来源：http://lvn.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ffa.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ycg.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkd.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crp.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vxe.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://ame.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fpc.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nrb.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://lkd.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sfy.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wzy.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oic.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rqu.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kzg.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jtw.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://gzb.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://orr.tian-w.cn

================================================================================
来源：http://qli.shzxlz.cn

F. 文件与目录
来源：http://flt.yonumen.top

================================================================================
来源：http://djd.xuetiantiany.cn

[F01] 读取整个文件
来源：http://tvg.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://phk.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://wub.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rvd.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xuq.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://spw.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wxg.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://hia.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://odj.mhx1999.top

[F02] 逐行读取文件
来源：http://pti.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rhc.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hez.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://slf.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xji.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://got.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lfd.aizwys.cn


<!-- 参考信息 -->