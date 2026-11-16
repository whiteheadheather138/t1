代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxh.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbl.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://doz.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://qnp.gaohongyu789.top

Ruby: arr.tally
来源：http://irl.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vjn.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://qjn.svipenyu.cn

Py:   x in arr
来源：http://fun.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://rnx.dashuyun.cn

JS:   arr.includes(x)
来源：http://xkv.tianlin.xyz

TS:   arr.includes(x)
来源：http://fvv.fengsongda.top

Java: list.contains(x)
来源：http://tnz.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://lrz.cashguo.top

Ruby: arr.include?(x)
来源：http://igu.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://cqq.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://xpa.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ufe.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://weh.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zea.yj20258888.top

TS:   [...arr];
来源：http://fhp.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://xat.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cvl.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://lyz.jinqigfzy.top

C#:   new List<int>(list);
来源：http://rno.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://kdx.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bba.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gnt.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vub.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ref.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://vfo.hcnkem.com

Go:   // 手写循环
来源：http://cpm.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dih.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wyp.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://nqy.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tww.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vnf.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://acz.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mnt.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://suo.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://urk.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gdc.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lln.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://kun.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lqr.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pnm.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gqv.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axu.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xiq.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ygm.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vlg.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zoh.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://djk.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://pxi.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://dfz.wangdashe.top

JS:   arr.join(", ")
来源：http://ffn.zdbjq.cn

TS:   arr.join(", ")
来源：http://ght.aizwys.cn

Java: String.join(", ", list)
来源：http://vsk.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://pfo.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://gjd.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://mjf.fanxiaobao.xyz

================================================================================
来源：http://wcf.smart0.xyz

E. 字符串处理
来源：http://loy.cdnleiting.top

================================================================================
来源：http://jcf.wangdashe.top

[E01] 拼接字符串
来源：http://jnl.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bfv.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mom.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfx.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hty.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ssl.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://krs.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://stb.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pgm.cheryme.top

[E02] 重复字符串
来源：http://kqw.sysykeji.top

Py:   "ab" * 3
来源：http://zvm.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://wes.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://syd.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://hyp.jiagoushi.top

Java: "ab".repeat(3)
来源：http://tbj.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://umq.sufxvd.cn

Ruby: "ab" * 3
来源：http://zjh.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kcz.fktsv.cn

[E03] 截取子串
来源：http://ljf.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gov.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yvb.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iov.epnwcf.com

TS:   s.slice(1, 4)
来源：http://ckt.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://uch.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ktf.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://tpv.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://zbd.zdbjq.cn

[E04] 查找子串位置
来源：http://gqq.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://mfp.xylfe.cn

PHP:  strpos($s, "x");
来源：http://nof.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gle.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://zbw.hcnkem.com

Java: s.indexOf("x")
来源：http://gch.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://mgw.pengpengdd.cyou

Ruby: s.index("x")
来源：http://nfq.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://qbj.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://elm.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ztc.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bbg.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxc.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://arj.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jnl.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rhx.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xnd.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wgt.chenzaomai.com

[E06] 替换子串
来源：http://cwy.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uhn.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://rdl.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eak.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://idy.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://org.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jth.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hva.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://ojh.fehbvm.com

[E07] 按分隔符拆分
来源：http://knb.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ufc.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://myh.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wdy.sjlbkw.cn

TS:   s.split(",")
来源：http://azu.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://mbl.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vvg.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://blv.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qfc.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://hmq.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://ndf.chenzaomai.com

PHP:  implode(",", $items);
来源：http://xnh.vqdsnc.cn

JS:   items.join(",")
来源：http://szx.zhoulong.xyz

TS:   items.join(",")
来源：http://mcy.gotoacloud.top

Java: String.join(",", items)
来源：http://wgy.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://kvo.sjlbkw.cn

Ruby: items.join(",")
来源：http://vyl.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://neg.hesvh.cn

[E09] 去除所有空白字符
来源：http://ucj.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iqo.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yxp.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://vba.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://dlp.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://rvc.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://nyz.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://jyz.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wrv.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://zal.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wnh.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kgu.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://ias.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://beg.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://qzk.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gke.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xrq.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hlx.pycfn.com

[E11] 反转字符串
来源：http://xyn.yvedp.cn

Py:   s[::-1]
来源：http://rvz.shzxlz.cn

PHP:  strrev($s);
来源：http://gdr.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://ktp.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://uoh.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://imh.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qlj.yfazqb.com

Ruby: s.reverse
来源：http://gtf.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://cwc.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://xmf.xinyue.icu

Py:   s.count("a")
来源：http://fgm.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://bfp.iojbl.cn

JS:   s.split("a").length - 1
来源：http://yvd.yueranfly.top

TS:   s.split("a").length - 1
来源：http://igh.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mcd.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://ves.hcnkem.com

Ruby: s.count("a")
来源：http://tol.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://rog.316326.xyz

[E13] 逐字符遍历
来源：http://xte.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://csz.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xxw.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://scg.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uwu.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rhu.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rfh.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jcd.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mjp.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://utw.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gej.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fdx.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afl.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://woj.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fpn.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sdk.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iom.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kyt.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://kft.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jzj.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wor.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bqs.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xvj.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qdx.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nmd.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nnt.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qvd.birdmap.top

[E16] 数字千分位
来源：http://yle.redwolf501.top

Py:   f"{1234567:,}"
来源：http://mff.yj20258.top

PHP:  number_format(1234567);
来源：http://snv.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://mil.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://njd.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lbb.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://owu.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lzz.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://and.dashuyun.cn

[E17] 首字母大写
来源：http://pkq.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hjv.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qzk.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rhz.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fxx.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pbh.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ijd.9152youxi.cn

Ruby: s.capitalize
来源：http://zvu.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nym.quarkkingdee.top

[E18] 模板占位符替换
来源：http://qhn.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tya.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yve.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eqn.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oyq.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vee.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vex.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kna.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vte.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://lah.cashguo.top

Py:   s.splitlines()
来源：http://tns.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rwb.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://kzn.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://dax.zhengqikj.top

Java: s.lines().toList()
来源：http://ujx.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://adp.daxiang520.top

Ruby: s.lines
来源：http://zes.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://pfi.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://jrn.fktsv.cn

Py:   if not s:
来源：http://udr.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hqc.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vfi.redwolf501.top

TS:   if (s === "") {}
来源：http://ekt.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://mnx.gaohongyu789.top

Go:   if s == "" {}
来源：http://jdd.zdbjq.cn

Ruby: if s.empty?
来源：http://ijb.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dgi.guowangkeji.top

[E21] 超长截断加省略号
来源：http://gbn.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vui.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhp.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://evo.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iwc.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxd.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://oye.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wwb.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hxj.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://uec.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wra.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnb.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjg.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ofo.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fld.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tfh.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://grw.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ssp.chenjidiqi.icu

================================================================================
来源：http://boo.fehbvm.com

F. 文件与目录
来源：http://hae.jqgufenzy.top

================================================================================
来源：http://ozx.hywenlv.cn

[F01] 读取整个文件
来源：http://eqn.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ifm.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://bic.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jca.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mjc.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ban.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sez.gzhubu.top

Ruby: File.read("a.txt")
来源：http://svu.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://vct.nwbrower.top

[F02] 逐行读取文件
来源：http://ikm.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nyc.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jry.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ipe.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmy.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzt.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rnx.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zwm.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjy.uphjek.com

[F03] 写入文件（覆盖）
来源：http://gdb.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tnj.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://osv.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://byp.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsu.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hcu.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ddh.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://zus.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://irl.yuxming.cn

[F04] 追加写入文件
来源：http://hvm.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tfs.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://djl.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sze.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tst.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qhu.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kij.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ste.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lxc.tarul.cn


<!-- 参考信息 -->