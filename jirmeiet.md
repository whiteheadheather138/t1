代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rqc.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sdt.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://ztl.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tgx.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bzg.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ude.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qbs.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://onx.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hnd.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qyr.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nny.ivvv.top

[D26] 数组转字符串
来源：http://enz.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://rqr.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://pto.sjlbkw.cn

JS:   arr.join(", ")
来源：http://akz.kuanghao11.cn

TS:   arr.join(", ")
来源：http://gex.jiagoushi.top

Java: String.join(", ", list)
来源：http://awk.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://loa.xylfe.cn

Ruby: arr.join(", ")
来源：http://bzj.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://bkl.zhoulong.xyz

================================================================================
来源：http://qbj.redwolf501.top

E. 字符串处理
来源：http://fes.jinghuilouyu.cn

================================================================================
来源：http://fwp.hnxiangtu.top

[E01] 拼接字符串
来源：http://rkk.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://krg.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ayp.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuk.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfv.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://esf.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://asp.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sby.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://njq.iojbl.cn

[E02] 重复字符串
来源：http://vxz.wangdashe.top

Py:   "ab" * 3
来源：http://vij.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://dte.fehbvm.com

JS:   "ab".repeat(3)
来源：http://upg.wangdashe.top

TS:   "ab".repeat(3)
来源：http://xzq.andypj.xyz

Java: "ab".repeat(3)
来源：http://fpn.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://lxu.hesvh.cn

Ruby: "ab" * 3
来源：http://wfy.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rkg.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://kwi.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://leh.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bpt.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cxy.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://qdy.hysaishi.cn

Java: s.substring(1, 4)
来源：http://dxi.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ndb.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://wlu.birdmap.top

C#:   s.Substring(1, 3)
来源：http://dkm.ctjpmb.com

[E04] 查找子串位置
来源：http://kcw.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://skf.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://zdb.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aoc.fzhhl.top

TS:   s.indexOf("x")
来源：http://knj.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://chk.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://qmb.hysaishi.cn

Ruby: s.index("x")
来源：http://jik.yonumen.top

C#:   s.IndexOf("x")
来源：http://noe.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ges.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ksn.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uuz.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtq.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mvq.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vnw.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://quu.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://whq.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyd.svipenyu.cn

[E06] 替换子串
来源：http://irv.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ayv.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://zke.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgl.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://hrt.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bdt.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://chu.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qeh.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://nwq.vehdjk.com

[E07] 按分隔符拆分
来源：http://tuf.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rnj.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ryw.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbi.jinghuilouyu.cn

TS:   s.split(",")
来源：http://wnc.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hbm.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bvb.ivvv.top

Ruby: s.split(",");  s.split
来源：http://eho.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://buz.gzhubu.top

[E08] 数组按分隔符合并
来源：http://xlf.fktsv.cn

Py:   ",".join(items)
来源：http://dnd.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://obn.aibaodan.cn

JS:   items.join(",")
来源：http://ket.smart0.xyz

TS:   items.join(",")
来源：http://muc.jiagoushi.top

Java: String.join(",", items)
来源：http://spy.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://gsp.andypj.xyz

Ruby: items.join(",")
来源：http://pym.ehwqpu.com

C#:   string.Join(",", items)
来源：http://azw.jianghu66.top

[E09] 去除所有空白字符
来源：http://mum.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fyh.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rra.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://qng.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://emy.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://hzt.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wgk.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wry.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rbu.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://ljc.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aih.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vsl.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://xfq.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://pfh.gzhubu.top

Java: String.format("%03d", 7)
来源：http://hog.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wzz.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lcm.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghx.chenlongwang.top

[E11] 反转字符串
来源：http://xgh.epnwcf.com

Py:   s[::-1]
来源：http://cnm.ivvv.top

PHP:  strrev($s);
来源：http://rgx.hammf.cn

JS:   [...s].reverse().join("")
来源：http://pef.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://ncw.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mat.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://xit.meibo888.top

Ruby: s.reverse
来源：http://pla.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ajo.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://wbe.cheryme.top

Py:   s.count("a")
来源：http://hku.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://ahb.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://joi.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://kxk.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pxh.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://wsl.cucudq.cn

Ruby: s.count("a")
来源：http://jzb.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://ftq.yongpay.top

[E13] 逐字符遍历
来源：http://tqg.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://xrt.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ytl.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://mri.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://raf.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oxl.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bbw.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wam.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nti.daxiang520.top

[E14] URL 编码与 Base64
来源：http://rua.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dbt.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zws.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xtf.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tpv.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cov.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bok.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kwy.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ipa.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://toj.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qhd.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qzl.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ejs.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sdh.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mbb.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hvf.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rlg.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://duu.jyoumei.cn

[E16] 数字千分位
来源：http://thn.mhx1999.top

Py:   f"{1234567:,}"
来源：http://rwg.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://evv.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jgj.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://znx.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wjc.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vxx.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zfc.ivvv.top

C#:   1234567.ToString("N0")
来源：http://xzg.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://qwp.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://edt.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kkq.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iag.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqg.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cot.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ixm.hfpthk.cn

Ruby: s.capitalize
来源：http://qjj.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tkt.hnqzz.top

[E18] 模板占位符替换
来源：http://cwc.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aht.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wkf.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lby.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qao.jinqigfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vsr.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zmd.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mvz.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fcg.yongpay.top

[E19] 多行文本按行拆分
来源：http://cgr.tian-w.cn

Py:   s.splitlines()
来源：http://qdb.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://svz.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://baj.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://thn.ctjpmb.com

Java: s.lines().toList()
来源：http://bjy.sweek.top

Go:   strings.Split(s, "\n")
来源：http://nmv.sufxvd.cn

Ruby: s.lines
来源：http://qvq.iojbl.cn

C#:   s.Split('\n')
来源：http://bly.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://dbx.mhx1999.top

Py:   if not s:
来源：http://lzc.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pgo.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rwk.vqdsnc.cn

TS:   if (s === "") {}
来源：http://duo.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://vwp.chenzaomai.com

Go:   if s == "" {}
来源：http://xrw.yj202588.top

Ruby: if s.empty?
来源：http://xxg.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iqn.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://vng.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yla.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mbw.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zux.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qgn.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bme.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://vxi.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://owg.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xol.pycfn.com

[E22] 字节长度与字符长度
来源：http://tbw.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bji.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibw.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjt.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xzx.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://txn.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ugl.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://xdg.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ylv.yfazqb.com

================================================================================
来源：http://dac.sweek.top

F. 文件与目录
来源：http://xmg.fengsongda.top

================================================================================
来源：http://pem.epnwcf.com

[F01] 读取整个文件
来源：http://srn.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zvu.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://tlz.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mlo.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cla.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://vol.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vpn.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://xpx.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://iqi.tianlin.xyz

[F02] 逐行读取文件
来源：http://nfm.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kuh.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vxb.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fca.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dqk.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xqp.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uof.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ebk.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgf.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://xce.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://odf.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://byj.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zgs.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnh.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ygy.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kud.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://uyu.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zib.bjfxy.top

[F04] 追加写入文件
来源：http://kil.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pvp.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cvp.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fat.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eio.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iyz.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ytr.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nmu.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nzs.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://uaz.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fwx.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://arh.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://ajx.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://fht.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bci.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sae.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://wtn.yonumen.top

C#:   File.Exists("a.txt")
来源：http://qmu.zhoulong.xyz

[F06] 删除文件
来源：http://ily.ybcxt.top

Py:   os.remove("a.txt")
来源：http://zqm.sxryk.cn

PHP:  unlink("a.txt");
来源：http://vwl.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rrp.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://soq.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jty.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://lyf.cheryme.top

Ruby: File.delete("a.txt")
来源：http://oxh.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://jbz.vehdjk.com

[F07] 创建目录（含多级）
来源：http://xzo.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fko.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cuq.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yos.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bec.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wlb.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iut.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://glu.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hzk.hnqzz.top

[F08] 遍历目录
来源：http://nkr.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rbe.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rkn.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://dzb.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://pzg.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqy.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://adx.hcnkem.com

Ruby: Dir.children("dir")
来源：http://kmw.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://ybl.zhengqikj.top

[F09] 获取文件大小
来源：http://pfb.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://jfr.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://aec.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://fsj.aibaodan.cn


<!-- 参考信息 -->