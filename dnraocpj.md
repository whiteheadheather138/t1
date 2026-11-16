代发 wailian999

Ruby: arr.tally
来源：http://ppy.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ati.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://uei.fktsv.cn

Py:   x in arr
来源：http://jgw.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://xyl.gogol.net.cn

JS:   arr.includes(x)
来源：http://dny.yvedp.cn

TS:   arr.includes(x)
来源：http://qto.aizwys.cn

Java: list.contains(x)
来源：http://ryy.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://cyq.jyoumei.cn

Ruby: arr.include?(x)
来源：http://chh.pycfn.com

C#:   list.Contains(x)
来源：http://luv.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://yir.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mii.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bfb.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ddl.sweek.top

TS:   [...arr];
来源：http://wja.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://jjf.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kia.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://zro.xylfe.cn

C#:   new List<int>(list);
来源：http://fgm.guowangkeji.top

[D23] reduce 累积计算
来源：http://utu.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mkg.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gyg.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mrk.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oce.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uej.tarul.cn

Go:   // 手写循环
来源：http://bqg.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gxz.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lpo.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://qct.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ins.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lrc.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hza.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbb.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xgl.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://exs.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oef.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jgm.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://dbo.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xaw.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://okc.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwn.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vkg.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aut.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xhl.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://swo.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://egt.vqdsnc.cn

[D26] 数组转字符串
来源：http://yfc.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://anc.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://rep.zhengqikj.top

JS:   arr.join(", ")
来源：http://prj.cucudq.cn

TS:   arr.join(", ")
来源：http://zkw.ppjwa.cn

Java: String.join(", ", list)
来源：http://ltc.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://ocp.yuxming.cn

Ruby: arr.join(", ")
来源：http://kdf.aizwys.cn

C#:   string.Join(", ", list)
来源：http://shm.316326.xyz

================================================================================
来源：http://xlu.zdqjudy.top

E. 字符串处理
来源：http://grv.hesvh.cn

================================================================================
来源：http://puj.shangyingyoupin.top

[E01] 拼接字符串
来源：http://yxm.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kge.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fwr.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hga.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nel.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcj.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aan.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hir.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://olv.jqgufenzy.top

[E02] 重复字符串
来源：http://odq.uphjek.com

Py:   "ab" * 3
来源：http://zmt.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://goc.cheryme.top

JS:   "ab".repeat(3)
来源：http://nqp.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://fyb.hysaishi.cn

Java: "ab".repeat(3)
来源：http://kww.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://knb.yongpay.top

Ruby: "ab" * 3
来源：http://aov.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eqw.kuanghao11.cn

[E03] 截取子串
来源：http://jbv.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mqs.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xir.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xye.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://qsk.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://aji.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://chy.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://bic.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://juf.dianchejie.cn

[E04] 查找子串位置
来源：http://jaw.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://hdk.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://tet.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eca.sysykeji.top

TS:   s.indexOf("x")
来源：http://not.jyoumei.cn

Java: s.indexOf("x")
来源：http://ycw.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://ktd.zdbjq.cn

Ruby: s.index("x")
来源：http://odl.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://nno.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://rox.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uvt.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zwp.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oay.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rto.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtb.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sit.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ace.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://svh.jqgufenzy.top

[E06] 替换子串
来源：http://ehj.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://afp.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://hoh.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ynm.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://dfo.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfo.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vaj.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iut.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://vax.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://yec.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rhe.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hdg.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://shb.yj20258888.top

TS:   s.split(",")
来源：http://yve.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://sxk.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tdo.sweek.top

Ruby: s.split(",");  s.split
来源：http://ixq.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qli.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://vkx.tianlin.xyz

Py:   ",".join(items)
来源：http://suw.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://tgh.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://vkb.shanyushiyangtech.top

TS:   items.join(",")
来源：http://nup.ivvv.top

Java: String.join(",", items)
来源：http://mjy.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://gwk.ehwqpu.com

Ruby: items.join(",")
来源：http://zfo.yj20258.top

C#:   string.Join(",", items)
来源：http://sog.yueranfly.top

[E09] 去除所有空白字符
来源：http://vhg.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjx.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dmb.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://she.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://isw.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://wrd.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://hxz.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://nlm.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://poo.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://sfk.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vls.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ujt.sweek.top

JS:   "7".padStart(3, "0")
来源：http://yfz.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://zff.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://nth.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gmr.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ajp.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dkf.jlsjyb.cn

[E11] 反转字符串
来源：http://par.yvedp.cn

Py:   s[::-1]
来源：http://ujw.nanxuanxn.top

PHP:  strrev($s);
来源：http://bor.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://dku.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://xmp.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jfk.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wxc.svipenyu.cn

Ruby: s.reverse
来源：http://uya.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://lve.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://wxh.cqqwz.cn

Py:   s.count("a")
来源：http://ejc.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://izs.fzhhl.top

JS:   s.split("a").length - 1
来源：http://rkk.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://wiw.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kww.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://huy.jinqigfzy.top

Ruby: s.count("a")
来源：http://zuy.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://dbj.xuanzx.com

[E13] 逐字符遍历
来源：http://jpi.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://uzm.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://law.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ier.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xbl.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zjc.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hsg.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mxt.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lhx.tarul.cn

[E14] URL 编码与 Base64
来源：http://jtz.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nni.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qqr.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://crv.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hfw.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://unf.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vyq.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zdf.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yte.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://res.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jit.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xxb.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fni.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gqx.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://brc.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://efo.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yhw.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xfj.shangyingyoupin.top

[E16] 数字千分位
来源：http://gqw.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://epk.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://urb.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oqd.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gnv.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ofa.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xsk.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vix.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://pyy.yonumen.top

[E17] 首字母大写
来源：http://nyf.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cvg.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ood.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://arl.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gjf.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://osw.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://muu.daxiang520.top

Ruby: s.capitalize
来源：http://ati.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hvu.gotoacloud.top

[E18] 模板占位符替换
来源：http://ujy.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qov.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oau.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lkb.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://phl.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dwc.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wrz.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cyt.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pbh.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://ike.svipenyu.cn

Py:   s.splitlines()
来源：http://ygj.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://plc.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://zet.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://gef.jqgufenzy.top

Java: s.lines().toList()
来源：http://pwr.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://orc.ywan-chungtsiang.top

Ruby: s.lines
来源：http://ixs.ppjwa.cn

C#:   s.Split('\n')
来源：http://sob.bbcook.cn

[E20] 判断字符串是否为空
来源：http://uwc.jlsjyb.cn

Py:   if not s:
来源：http://eri.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uiy.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qko.snrcjt.cn

TS:   if (s === "") {}
来源：http://ybe.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://vwh.cucudq.cn

Go:   if s == "" {}
来源：http://ati.yonumen.top

Ruby: if s.empty?
来源：http://cdk.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://swi.shuidangran.top

[E21] 超长截断加省略号
来源：http://ygt.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kfe.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://axg.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkz.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ziv.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wmx.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://mqt.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nwn.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lun.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://xxw.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hir.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsa.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqv.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyk.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://olc.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://njk.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://sqw.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xgw.andypj.xyz

================================================================================
来源：http://oql.zhixingplan.top

F. 文件与目录
来源：http://xyc.shuidangran.top

================================================================================
来源：http://cjt.cucudq.cn

[F01] 读取整个文件
来源：http://xxx.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://whc.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://lia.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hjz.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xaw.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wmz.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bqp.zycfv.cn

Ruby: File.read("a.txt")
来源：http://rpd.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://qrl.aizwys.cn

[F02] 逐行读取文件
来源：http://kyp.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jxu.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://opa.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fav.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbc.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzp.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gaj.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://itg.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ygx.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://hht.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wlr.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rtj.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://exr.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjd.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kdn.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vwp.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://yfy.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vri.hnxiangtu.top

[F04] 追加写入文件
来源：http://zon.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uiu.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ceq.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxg.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwd.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hns.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://adi.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mub.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://khl.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://ili.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://etb.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://dnd.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://vqy.ydzc1.top


<!-- 参考信息 -->