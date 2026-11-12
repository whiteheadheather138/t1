代发 wailian999

Java: String.join(", ", list)
来源：http://ekr.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://opo.haohaochexian.top

Ruby: arr.join(", ")
来源：http://ruz.hcnkem.com

C#:   string.Join(", ", list)
来源：http://ekm.316326.xyz

================================================================================
来源：http://psd.kuanghao11.cn

E. 字符串处理
来源：http://jrr.hesvh.cn

================================================================================
来源：http://tfj.hysaishi.cn

[E01] 拼接字符串
来源：http://ncd.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rqi.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hhe.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bxy.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qip.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yzs.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uvf.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bao.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdw.ehwqpu.com

[E02] 重复字符串
来源：http://exi.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://uyk.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://jpw.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://hpo.xziqi.cn

TS:   "ab".repeat(3)
来源：http://ysw.yuxming.cn

Java: "ab".repeat(3)
来源：http://orz.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://wjo.ivvv.top

Ruby: "ab" * 3
来源：http://uad.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://epp.zycfv.cn

[E03] 截取子串
来源：http://tof.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wne.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cjv.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mrz.nwbrower.top

TS:   s.slice(1, 4)
来源：http://fym.yj20258.top

Java: s.substring(1, 4)
来源：http://fhk.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bkk.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bfw.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://fbz.yj20258888.top

[E04] 查找子串位置
来源：http://unc.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://lub.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://tqg.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://urc.daria6918.cn

TS:   s.indexOf("x")
来源：http://ohz.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://hgk.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://uce.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://ioy.fzhhl.top

C#:   s.IndexOf("x")
来源：http://vfo.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://alw.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ihq.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hka.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djd.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xtg.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rqf.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gsd.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mhd.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://akt.bbcook.cn

[E06] 替换子串
来源：http://bae.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://djq.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://vjr.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayy.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://rxf.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yrb.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wnv.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ljq.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://niq.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://pwc.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hsq.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrd.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://scl.pycfn.com

TS:   s.split(",")
来源：http://wdt.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://bgj.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nsl.yonumen.top

Ruby: s.split(",");  s.split
来源：http://hao.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xtl.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://gwf.jqgufenzy.top

Py:   ",".join(items)
来源：http://dby.yj202588.top

PHP:  implode(",", $items);
来源：http://iix.yongpay.top

JS:   items.join(",")
来源：http://zkx.ppjwa.cn

TS:   items.join(",")
来源：http://fck.iojbl.cn

Java: String.join(",", items)
来源：http://yyi.yongpay.top

Go:   strings.Join(items, ",")
来源：http://jho.52xcode.cn

Ruby: items.join(",")
来源：http://pre.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://aku.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://czj.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://plw.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cry.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://sjw.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://yjw.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://ktn.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pmz.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://yyu.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xjh.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://hau.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vga.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://unz.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://uuy.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://qbc.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://bwe.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pdk.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ctg.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ktg.gogol.net.cn

[E11] 反转字符串
来源：http://kvb.bjfxy.top

Py:   s[::-1]
来源：http://uzo.iojbl.cn

PHP:  strrev($s);
来源：http://qnp.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://bou.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://esq.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ddf.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ngm.gogol.net.cn

Ruby: s.reverse
来源：http://uhf.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zdr.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://zee.quarkkingdee.top

Py:   s.count("a")
来源：http://uze.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://upu.yvedp.cn

JS:   s.split("a").length - 1
来源：http://bvd.ydzc1.top

TS:   s.split("a").length - 1
来源：http://cpp.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dyh.uphjek.com

Go:   strings.Count(s, "a")
来源：http://pnm.ybcxt.top

Ruby: s.count("a")
来源：http://nzb.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://zyp.tanke756.top

[E13] 逐字符遍历
来源：http://xuw.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://zhw.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tvh.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://brt.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lss.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wwp.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dnu.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://olx.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gnx.316326.xyz

[E14] URL 编码与 Base64
来源：http://eun.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mgu.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://epl.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nyp.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mbf.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ssa.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jnn.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iwj.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obk.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://zvj.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lum.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uzf.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yjf.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ioy.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcm.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ytu.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lxd.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mjp.uphjek.com

[E16] 数字千分位
来源：http://dpl.hammf.cn

Py:   f"{1234567:,}"
来源：http://ahb.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://bfo.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zgc.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ljh.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cot.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pve.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gat.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://sjm.hysaishi.cn

[E17] 首字母大写
来源：http://mre.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gjl.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbh.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fiu.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqi.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xyd.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fdg.fehbvm.com

Ruby: s.capitalize
来源：http://jnd.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bck.smart0.xyz

[E18] 模板占位符替换
来源：http://csm.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yia.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mwp.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vwp.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lef.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jof.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uvr.bbcook.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://leg.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://feo.hcnkem.com

[E19] 多行文本按行拆分
来源：http://djv.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://jfp.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dvs.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://lyj.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://fyb.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://gkp.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://sww.hongshengwenyu.top

Ruby: s.lines
来源：http://uhc.iojbl.cn

C#:   s.Split('\n')
来源：http://knd.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://wtu.fengsongda.top

Py:   if not s:
来源：http://bqa.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qbh.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rte.yuanzhike.top

TS:   if (s === "") {}
来源：http://npp.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://chs.zycfv.cn

Go:   if s == "" {}
来源：http://zfy.tarul.cn

Ruby: if s.empty?
来源：http://vya.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mow.snrcjt.cn

[E21] 超长截断加省略号
来源：http://jqu.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wxe.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dej.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cjk.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cqd.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://upd.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://mox.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qok.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ikz.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://cpi.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://umk.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tsu.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xom.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ewo.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://egp.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jnh.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://bwn.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uij.snrcjt.cn

================================================================================
来源：http://uaa.dianchejie.cn

F. 文件与目录
来源：http://gad.sysykeji.top

================================================================================
来源：http://rbf.fehbvm.com

[F01] 读取整个文件
来源：http://vmm.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xru.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://vxh.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqu.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ftg.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kmp.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wil.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://yha.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://dsv.wangdashe.top

[F02] 逐行读取文件
来源：http://awi.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lrs.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ljg.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwt.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qlb.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://atc.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://abd.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nqr.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fhc.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://jua.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rqt.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://afa.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihb.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oac.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zwr.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ylx.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://yyh.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iiv.hysaishi.cn

[F04] 追加写入文件
来源：http://hqp.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xzz.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://foy.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpa.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mur.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rdf.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iga.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pob.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://alm.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://ncj.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nao.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://jsu.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://bkx.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://ham.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kuv.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zoo.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://ife.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://wqr.shuidangran.top

[F06] 删除文件
来源：http://fyi.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://nzp.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://fil.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://nql.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://awi.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ftb.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://oxq.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://azl.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://jbf.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://wsi.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gmv.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yli.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vsm.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tun.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://krc.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pkg.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mek.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zex.vehdjk.com

[F08] 遍历目录
来源：http://cgx.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aje.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nni.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://hnk.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://wcg.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dtc.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://clf.yueranfly.top

Ruby: Dir.children("dir")
来源：http://qrv.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://xrm.birdmap.top

[F09] 获取文件大小
来源：http://gao.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://hta.fzhhl.top

PHP:  filesize("a.txt");
来源：http://hrc.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://yfn.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://zrw.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xoj.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zwc.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://gya.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://hzj.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://ziy.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tvl.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kpw.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://reh.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://ncp.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wpq.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yyh.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fyl.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dri.tian-w.cn

[F11] 复制与移动文件
来源：http://hsw.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tzx.52xcode.cn


<!-- 参考信息 -->