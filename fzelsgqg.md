代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://ysv.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xsk.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://olg.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://chp.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ozy.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://zag.cucudq.cn

Py:   Counter(arr)
来源：http://tbc.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://obj.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvz.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrs.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://igk.hcnkem.com

Go:   // 手写 map[T]int
来源：http://eyc.cqqwz.cn

Ruby: arr.tally
来源：http://ecg.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wtf.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://xej.jiagoushi.top

Py:   x in arr
来源：http://qaq.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://pyi.gogol.net.cn

JS:   arr.includes(x)
来源：http://yxt.snrcjt.cn

TS:   arr.includes(x)
来源：http://fww.meibo888.top

Java: list.contains(x)
来源：http://wtf.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://bys.nanxinkj.top

Ruby: arr.include?(x)
来源：http://ywg.jqgfzy.top

C#:   list.Contains(x)
来源：http://hiw.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://ebk.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fjg.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jrn.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ohb.hesvh.cn

TS:   [...arr];
来源：http://ekb.cheryme.top

Java: new ArrayList<>(list);
来源：http://ryg.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://vaz.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://nnu.gzhubu.top

C#:   new List<int>(list);
来源：http://ixa.andypj.xyz

[D23] reduce 累积计算
来源：http://rfy.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vcx.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hdr.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgh.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://coy.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zre.pycfn.com

Go:   // 手写循环
来源：http://krm.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mng.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jig.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://kjr.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cet.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://knm.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rnt.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ngm.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xcq.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mgt.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kxh.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hri.cashguo.top

[D25] Set 集合去重与交并差
来源：http://tzo.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ygo.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dhz.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ifx.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dwz.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bry.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ccq.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pzx.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hti.jqgfzy.top

[D26] 数组转字符串
来源：http://mxy.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://non.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://fcs.jianghu66.top

JS:   arr.join(", ")
来源：http://yct.bbcook.cn

TS:   arr.join(", ")
来源：http://xsi.ivvv.top

Java: String.join(", ", list)
来源：http://fhd.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://yrh.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://xfr.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://wes.epnwcf.com

================================================================================
来源：http://yts.ehwqpu.com

E. 字符串处理
来源：http://hru.hammf.cn

================================================================================
来源：http://ugq.cucudq.cn

[E01] 拼接字符串
来源：http://ixr.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iiy.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bwj.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://akr.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pmd.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wba.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ful.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xcq.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nxe.zdbjq.cn

[E02] 重复字符串
来源：http://rhv.ivvv.top

Py:   "ab" * 3
来源：http://bhw.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://dyh.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://dpr.guannengcc.top

TS:   "ab".repeat(3)
来源：http://ras.yvedp.cn

Java: "ab".repeat(3)
来源：http://hwo.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://ljo.zdqjudy.top

Ruby: "ab" * 3
来源：http://obd.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://slv.mhx1999.top

[E03] 截取子串
来源：http://puv.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqp.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jti.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rkj.ybcxt.top

TS:   s.slice(1, 4)
来源：http://kjz.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://vva.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://phy.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lpw.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://mee.gotoacloud.top

[E04] 查找子串位置
来源：http://frx.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://voh.yj20258.top

PHP:  strpos($s, "x");
来源：http://kyq.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eqy.daxiang520.top

TS:   s.indexOf("x")
来源：http://emx.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://kbk.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://vzm.fengsongda.top

Ruby: s.index("x")
来源：http://eek.jianghu66.top

C#:   s.IndexOf("x")
来源：http://ikb.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ztr.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcf.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jhk.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wds.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xuw.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sgm.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fzy.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eeo.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://grv.haohaochexian.top

[E06] 替换子串
来源：http://dxv.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qkh.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://lxl.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bql.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://ylc.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpq.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ahf.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dfm.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://ihe.ppjwa.cn

[E07] 按分隔符拆分
来源：http://ybf.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mpb.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zhs.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ude.tanke756.top

TS:   s.split(",")
来源：http://aoc.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://vxo.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zkd.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://pez.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lew.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://nyi.yueranfly.top

Py:   ",".join(items)
来源：http://zin.wangdashe.top

PHP:  implode(",", $items);
来源：http://plr.yueranfly.top

JS:   items.join(",")
来源：http://yem.quarkkingdee.top

TS:   items.join(",")
来源：http://gvu.tian-w.cn

Java: String.join(",", items)
来源：http://xsj.yonumen.top

Go:   strings.Join(items, ",")
来源：http://ute.pycfn.com

Ruby: items.join(",")
来源：http://anq.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://czs.yj20258.top

[E09] 去除所有空白字符
来源：http://xjy.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wnf.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vxx.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://yem.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://xoc.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://yrr.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pyv.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://tqa.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dbm.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://ina.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bqm.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uke.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://zcj.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://kdk.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://ppz.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ucb.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ust.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejm.jinqigfzy.top

[E11] 反转字符串
来源：http://gfa.jinqigufen.top

Py:   s[::-1]
来源：http://mzt.xinyue.icu

PHP:  strrev($s);
来源：http://zks.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://hsg.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://xnn.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qqw.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lkq.yj20258.top

Ruby: s.reverse
来源：http://kls.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nth.yueranfly.top

[E12] 统计某字符出现次数
来源：http://tnw.cdnleiting.top

Py:   s.count("a")
来源：http://kvu.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://tbs.bbcook.cn

JS:   s.split("a").length - 1
来源：http://hhy.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://bqe.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bel.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://oxi.yangfankeji.com

Ruby: s.count("a")
来源：http://yij.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://bbd.sysykeji.top

[E13] 逐字符遍历
来源：http://blj.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://exo.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mrn.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ioy.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wru.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brh.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://apo.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://hrt.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ytd.nwbrower.top

[E14] URL 编码与 Base64
来源：http://jwp.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://auz.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xya.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yrm.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rop.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xik.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gqb.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://agd.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xvx.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://ejc.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uab.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aud.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ahe.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zbm.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rey.xylfe.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fml.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sqo.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://juv.hammf.cn

[E16] 数字千分位
来源：http://mwg.fzhhl.top

Py:   f"{1234567:,}"
来源：http://nuq.sufxvd.cn

PHP:  number_format(1234567);
来源：http://pwg.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qvh.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xvq.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqo.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ltr.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gak.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://jmi.gotoacloud.top

[E17] 首字母大写
来源：http://kjs.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://afg.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://olh.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://orm.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vka.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qax.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xco.mhx1999.top

Ruby: s.capitalize
来源：http://amk.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gqw.jiagoushi.top

[E18] 模板占位符替换
来源：http://tuw.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uew.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gfx.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tgh.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ejc.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rgl.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pad.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ksg.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xsx.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://hnf.cucudq.cn

Py:   s.splitlines()
来源：http://fnf.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://phq.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://jqi.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://owm.jqgufenzy.top

Java: s.lines().toList()
来源：http://joo.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://vzc.yvedp.cn

Ruby: s.lines
来源：http://lkr.yj202588.top

C#:   s.Split('\n')
来源：http://khb.hnqzz.top

[E20] 判断字符串是否为空
来源：http://cpf.tian-w.cn

Py:   if not s:
来源：http://bsc.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zaq.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nwi.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://sca.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://npk.mhx1999.top

Go:   if s == "" {}
来源：http://tpd.tian-w.cn

Ruby: if s.empty?
来源：http://igj.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dlj.vehdjk.com

[E21] 超长截断加省略号
来源：http://ich.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cbb.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qsa.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://awk.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qxb.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://srq.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://szf.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cjx.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rcb.hcnkem.com

[E22] 字节长度与字符长度
来源：http://cbx.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qgx.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hmm.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxa.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lun.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lkf.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xde.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://efq.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://frj.jinqigfzy.top

================================================================================
来源：http://vub.yj20258888.top

F. 文件与目录
来源：http://nqx.ctjpmb.com

================================================================================
来源：http://vle.zycfv.cn

[F01] 读取整个文件
来源：http://mvz.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ixj.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://xtm.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ssv.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lrr.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://erk.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nnw.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://dcl.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://cxo.dianchejie.cn

[F02] 逐行读取文件
来源：http://pqp.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cip.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dgy.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iks.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://taz.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dge.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xtc.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://djc.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://upj.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://jqz.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kod.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fci.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sru.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhe.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://waj.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zjh.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://wel.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://emc.meibo888.top

[F04] 追加写入文件
来源：http://rea.c1oappe.top


<!-- 参考信息 -->