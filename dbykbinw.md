代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://xrc.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://ttf.haohaochexian.top

JS:   arr.join(", ")
来源：http://lya.yangfankeji.com

TS:   arr.join(", ")
来源：http://mxb.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://arv.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://shq.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://qgh.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://byc.nwbrower.top

================================================================================
来源：http://gum.haohaochexian.top

E. 字符串处理
来源：http://kwz.dianchejie.cn

================================================================================
来源：http://udw.hcnkem.com

[E01] 拼接字符串
来源：http://rwe.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gsz.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vlf.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppr.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dwu.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uym.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdy.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gkn.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ldw.ybcxt.top

[E02] 重复字符串
来源：http://jkq.fktsv.cn

Py:   "ab" * 3
来源：http://amj.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://qrx.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://edh.shuidangran.top

TS:   "ab".repeat(3)
来源：http://nhx.hammf.cn

Java: "ab".repeat(3)
来源：http://ytg.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://gxn.hcnkem.com

Ruby: "ab" * 3
来源：http://voc.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjy.chenzaomai.com

[E03] 截取子串
来源：http://wxl.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wzw.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kfk.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rfx.sysykeji.top

TS:   s.slice(1, 4)
来源：http://gle.yj20258888.top

Java: s.substring(1, 4)
来源：http://pzs.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://far.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xsl.pycfn.com

C#:   s.Substring(1, 3)
来源：http://lkc.yueranfly.top

[E04] 查找子串位置
来源：http://doa.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://zfa.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://qsc.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uct.cucudq.cn

TS:   s.indexOf("x")
来源：http://vnb.zhijiandao.cn

Java: s.indexOf("x")
来源：http://bah.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://axx.yuxming.cn

Ruby: s.index("x")
来源：http://ssl.yueranfly.top

C#:   s.IndexOf("x")
来源：http://jbw.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hto.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xub.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsa.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fod.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ijm.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ocg.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pch.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vxi.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ptq.316326.xyz

[E06] 替换子串
来源：http://zrs.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sxm.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://cwp.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjr.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://rht.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://svg.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zga.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hch.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://tpj.sweek.top

[E07] 按分隔符拆分
来源：http://ojy.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sxk.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nim.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktg.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://owl.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://vkt.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lqe.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://kks.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tlh.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://uce.havefunace.top

Py:   ",".join(items)
来源：http://viq.birdmap.top

PHP:  implode(",", $items);
来源：http://msn.wangshuangyany.cn

JS:   items.join(",")
来源：http://xcw.gogol.net.cn

TS:   items.join(",")
来源：http://ieh.meibo888.top

Java: String.join(",", items)
来源：http://dwr.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://avk.uphjek.com

Ruby: items.join(",")
来源：http://qmf.andypj.xyz

C#:   string.Join(",", items)
来源：http://lhz.zdbjq.cn

[E09] 去除所有空白字符
来源：http://pkg.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://odv.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zgv.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://gse.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://cva.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://oii.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://efl.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://bbq.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqz.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://wkj.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rfv.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fub.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://ykr.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://rdv.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://shc.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ios.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://psj.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hck.yonumen.top

[E11] 反转字符串
来源：http://zzz.svipenyu.cn

Py:   s[::-1]
来源：http://kax.smart0.xyz

PHP:  strrev($s);
来源：http://viy.pycfn.com

JS:   [...s].reverse().join("")
来源：http://bpi.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://nzu.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sok.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hgn.yj20258888.top

Ruby: s.reverse
来源：http://fhw.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pfv.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://yor.hongshengwenyu.top

Py:   s.count("a")
来源：http://ldf.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://brg.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://idk.yonumen.top

TS:   s.split("a").length - 1
来源：http://bwp.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fdt.pycfn.com

Go:   strings.Count(s, "a")
来源：http://rkr.nanxuanxn.top

Ruby: s.count("a")
来源：http://gxq.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://vjo.yj20258888.top

[E13] 逐字符遍历
来源：http://bcy.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://svv.cheryme.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xhp.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hwt.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qhg.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qml.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jfm.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ymc.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oas.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://gxq.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pvv.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://spb.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kvk.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rqh.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://djt.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dch.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xjp.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mfq.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://zse.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mlt.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ptw.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uvi.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://wuz.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rhy.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://klv.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cnb.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tlc.c1oappe.top

[E16] 数字千分位
来源：http://dzx.shuidangran.top

Py:   f"{1234567:,}"
来源：http://jbw.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://qzt.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rxq.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zib.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fiy.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uad.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ztn.316326.xyz

C#:   1234567.ToString("N0")
来源：http://dfw.zhijiandao.cn

[E17] 首字母大写
来源：http://fbj.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qoi.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vfd.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ldu.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyw.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jtc.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mkc.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://akm.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eym.fktsv.cn

[E18] 模板占位符替换
来源：http://cdm.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gzh.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mtp.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lze.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jza.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zjf.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yvn.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dtc.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dha.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://lhg.zdbjq.cn

Py:   s.splitlines()
来源：http://wrd.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://asm.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://auf.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://icf.yj20258.top

Java: s.lines().toList()
来源：http://lul.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://exx.yuanzhike.top

Ruby: s.lines
来源：http://xsd.ybcxt.top

C#:   s.Split('\n')
来源：http://lpm.vehdjk.com

[E20] 判断字符串是否为空
来源：http://oup.xinyue.icu

Py:   if not s:
来源：http://ovj.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibv.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kau.yuanzhike.top

TS:   if (s === "") {}
来源：http://hbq.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://ghm.pengpengdd.cyou

Go:   if s == "" {}
来源：http://wig.xinyue.icu

Ruby: if s.empty?
来源：http://lqq.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eky.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://bum.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lrz.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://spu.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bit.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyv.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tnb.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://ufo.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dmu.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tac.havefunace.top

[E22] 字节长度与字符长度
来源：http://sgu.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ech.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xih.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sze.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nkv.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fie.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oww.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://lkl.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vxa.nanxuanxn.top

================================================================================
来源：http://snk.vqdsnc.cn

F. 文件与目录
来源：http://woo.sjlbkw.cn

================================================================================
来源：http://kwa.gaohongyu789.top

[F01] 读取整个文件
来源：http://kxl.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zwd.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://dqc.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lew.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjd.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fca.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lkt.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://ivz.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://pwc.wangdashe.top

[F02] 逐行读取文件
来源：http://ekt.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qls.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nle.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yin.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pav.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qkt.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yhd.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fqa.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://huo.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://bjm.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tif.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zwx.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qzp.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ekx.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wgi.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ylf.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://rcw.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sva.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://yvx.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ccz.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gvk.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qke.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqx.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jhg.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sca.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tpp.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fsg.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://dzy.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wvc.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://jku.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://uqe.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://des.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ffc.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dxt.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://ypl.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://ncs.jinghuilouyu.cn

[F06] 删除文件
来源：http://ymy.zycfv.cn

Py:   os.remove("a.txt")
来源：http://icb.ybcxt.top

PHP:  unlink("a.txt");
来源：http://mqa.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://sps.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://ijy.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dmu.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://ysb.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://ebe.pycfn.com

C#:   File.Delete("a.txt");
来源：http://rjz.hesvh.cn

[F07] 创建目录（含多级）
来源：http://xku.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bus.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://icy.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://col.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bbl.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tvs.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qgz.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ooc.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qjq.yj20258888.top

[F08] 遍历目录
来源：http://crv.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://liv.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rrn.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://pov.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://gdm.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://itz.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nlx.cashguo.top

Ruby: Dir.children("dir")
来源：http://lmt.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://ecw.jqgufenzy.top

[F09] 获取文件大小
来源：http://lcr.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://lpo.vehdjk.com

PHP:  filesize("a.txt");
来源：http://ngy.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://six.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://thd.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lkp.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lgz.fengsongda.top

Ruby: File.size("a.txt")
来源：http://exm.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://ibp.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://lph.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cyc.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vaf.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kja.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://cft.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rga.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mxx.gogol.net.cn


<!-- 参考信息 -->