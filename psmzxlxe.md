代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://pfj.zhixingplan.top

JS:   arr.includes(x)
来源：http://byd.ctjpmb.com

TS:   arr.includes(x)
来源：http://umi.aibaodan.cn

Java: list.contains(x)
来源：http://cvb.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://fsr.316326.xyz

Ruby: arr.include?(x)
来源：http://wme.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://ztg.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://pik.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bzc.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://irv.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lih.chenjidiqi.icu

TS:   [...arr];
来源：http://myi.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://ozy.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uvw.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://zkw.hnxiangtu.top

C#:   new List<int>(list);
来源：http://gbe.snrcjt.cn

[D23] reduce 累积计算
来源：http://hao.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hpd.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zoz.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thw.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xzq.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://smj.cashguo.top

Go:   // 手写循环
来源：http://jby.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://idv.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://huq.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://nby.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://izb.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://biy.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pub.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hjq.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ldf.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bwz.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sjk.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kzw.yonumen.top

[D25] Set 集合去重与交并差
来源：http://ffd.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwp.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bvm.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dvv.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://inl.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mld.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cid.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gzw.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://boz.sufxvd.cn

[D26] 数组转字符串
来源：http://pnq.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://gre.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://ike.tianlin.xyz

JS:   arr.join(", ")
来源：http://krp.nanxinkj.top

TS:   arr.join(", ")
来源：http://bjj.xziqi.cn

Java: String.join(", ", list)
来源：http://vdb.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://vae.jiagoushi.top

Ruby: arr.join(", ")
来源：http://fpf.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://pen.quarkkingdee.top

================================================================================
来源：http://kfc.yj202588.top

E. 字符串处理
来源：http://icj.sjlbkw.cn

================================================================================
来源：http://tts.jianghu66.top

[E01] 拼接字符串
来源：http://qpj.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hsn.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://suc.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sve.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fce.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uwm.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://icw.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://byw.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ixv.nanxuanxn.top

[E02] 重复字符串
来源：http://eyy.hnqzz.top

Py:   "ab" * 3
来源：http://kpo.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://pir.tarul.cn

JS:   "ab".repeat(3)
来源：http://dej.daria6918.cn

TS:   "ab".repeat(3)
来源：http://jwe.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://cbe.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bhj.bbcook.cn

Ruby: "ab" * 3
来源：http://qpw.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kac.fktsv.cn

[E03] 截取子串
来源：http://bhu.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jhv.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iew.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvx.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://kme.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://nrf.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://flj.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://spn.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://ulg.9152youxi.cn

[E04] 查找子串位置
来源：http://swj.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://uvk.birdmap.top

PHP:  strpos($s, "x");
来源：http://yxh.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ddh.andypj.xyz

TS:   s.indexOf("x")
来源：http://qop.xinyue.icu

Java: s.indexOf("x")
来源：http://tin.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://hxi.aizwys.cn

Ruby: s.index("x")
来源：http://bon.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://lwm.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mfl.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqh.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ydw.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eqr.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tgs.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sae.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yyh.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://umd.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wuy.yonumen.top

[E06] 替换子串
来源：http://kgu.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xcr.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://yhw.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pkm.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://upi.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yyx.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vsf.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://klf.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://xna.fktsv.cn

[E07] 按分隔符拆分
来源：http://olw.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pms.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rlu.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fqe.yvedp.cn

TS:   s.split(",")
来源：http://qjx.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://jup.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nfn.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://cfv.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://asj.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://rbz.chenlongwang.top

Py:   ",".join(items)
来源：http://ydd.gogol.net.cn

PHP:  implode(",", $items);
来源：http://amg.fengsongda.top

JS:   items.join(",")
来源：http://cbc.epnwcf.com

TS:   items.join(",")
来源：http://yvc.sufxvd.cn

Java: String.join(",", items)
来源：http://abf.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://bcp.nanxinkj.top

Ruby: items.join(",")
来源：http://xau.uphjek.com

C#:   string.Join(",", items)
来源：http://mnl.iojbl.cn

[E09] 去除所有空白字符
来源：http://kgw.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxq.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fah.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://exg.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://lvc.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://pfz.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zrt.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://fde.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oem.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://ach.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fdz.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tjp.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://fxh.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://btq.bjfxy.top

Java: String.format("%03d", 7)
来源：http://coh.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yti.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pdz.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vko.birdmap.top

[E11] 反转字符串
来源：http://njq.tarul.cn

Py:   s[::-1]
来源：http://ydp.yanxiufei.cn

PHP:  strrev($s);
来源：http://hvf.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://kzl.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://yfc.gaohongyu789.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mhh.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ynj.zdqjudy.top

Ruby: s.reverse
来源：http://pvn.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uab.daria6918.cn

[E12] 统计某字符出现次数
来源：http://bxg.pycfn.com

Py:   s.count("a")
来源：http://lkr.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://szh.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://ltl.pycfn.com

TS:   s.split("a").length - 1
来源：http://lij.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gwb.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://rqq.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://ihb.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://ixy.bbcook.cn

[E13] 逐字符遍历
来源：http://jld.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://kxg.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lug.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://npr.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hyr.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rfb.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://faq.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ouc.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wmv.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://izh.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://njw.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qpe.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tvl.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uus.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dqs.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iyv.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fnq.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzy.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://rqh.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://cnb.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xed.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://arp.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dea.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ujz.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mav.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iyl.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gms.cashguo.top

[E16] 数字千分位
来源：http://tld.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://pxh.cqqwz.cn

PHP:  number_format(1234567);
来源：http://gbk.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ggr.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lcf.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ouh.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayr.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kts.yonumen.top

C#:   1234567.ToString("N0")
来源：http://xtl.9152youxi.cn

[E17] 首字母大写
来源：http://dld.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xsn.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnp.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mct.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbb.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tqf.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iki.gotoacloud.top

Ruby: s.capitalize
来源：http://lig.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wwg.zhijiandao.cn

[E18] 模板占位符替换
来源：http://auy.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://azf.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lwx.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bqz.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ggg.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hac.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zoh.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yqm.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zfb.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://ggo.gogol.net.cn

Py:   s.splitlines()
来源：http://slt.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://res.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://lpb.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://eot.yvedp.cn

Java: s.lines().toList()
来源：http://hud.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://oql.0kj1m.cn

Ruby: s.lines
来源：http://pzg.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://bib.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://pdo.jinyuanbaomall.cn

Py:   if not s:
来源：http://jkb.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cxe.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qav.316326.xyz

TS:   if (s === "") {}
来源：http://cqp.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://mys.xuetiantiany.cn

Go:   if s == "" {}
来源：http://cgr.daria6918.cn

Ruby: if s.empty?
来源：http://hog.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hdp.guowangkeji.top

[E21] 超长截断加省略号
来源：http://guw.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pwx.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhg.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ept.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgs.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bby.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://hcj.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hdm.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ecn.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://ekp.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sgt.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vob.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhc.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rda.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ddu.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lct.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://alp.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bop.epnwcf.com

================================================================================
来源：http://ulo.fengsongda.top

F. 文件与目录
来源：http://vca.epnwcf.com

================================================================================
来源：http://psh.yuxming.cn

[F01] 读取整个文件
来源：http://imr.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vpc.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://yye.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ycx.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://flq.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://asw.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hsv.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://psv.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://ssj.shzxlz.cn

[F02] 逐行读取文件
来源：http://rpg.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gfi.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cxj.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bxj.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wbs.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lqb.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vic.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tut.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ztv.sweek.top

[F03] 写入文件（覆盖）
来源：http://iok.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aec.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbl.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpr.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pbt.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://njg.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kyg.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://cyn.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://egk.tanke756.top

[F04] 追加写入文件
来源：http://rxq.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mak.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ogk.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nxs.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gaz.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jnq.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhm.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rfx.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xof.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://une.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cqm.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://swt.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://ryk.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://oob.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kmd.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tbl.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://uaa.cashguo.top


<!-- 参考信息 -->