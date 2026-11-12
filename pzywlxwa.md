代发 wailian999

Java: String.join(", ", list)
来源：http://wzt.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://zwu.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://wqj.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://sog.ybcxt.top

================================================================================
来源：http://cby.nanxinkj.top

E. 字符串处理
来源：http://ncv.c1oappe.top

================================================================================
来源：http://oqn.iojbl.cn

[E01] 拼接字符串
来源：http://xin.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eyh.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pvy.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kgl.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pdh.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wcl.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cba.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://prn.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tim.dianchejie.cn

[E02] 重复字符串
来源：http://dqb.smart0.xyz

Py:   "ab" * 3
来源：http://tts.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://dkc.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://mjo.fktsv.cn

TS:   "ab".repeat(3)
来源：http://sln.zhixingplan.top

Java: "ab".repeat(3)
来源：http://bvb.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://frx.daxiang520.top

Ruby: "ab" * 3
来源：http://khe.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pdk.cqqwz.cn

[E03] 截取子串
来源：http://ear.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zqd.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sad.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fjt.hnqzz.top

TS:   s.slice(1, 4)
来源：http://ezj.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://cin.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xot.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://zrc.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://upb.redwolf501.top

[E04] 查找子串位置
来源：http://yov.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://jxs.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://dou.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pxz.tianlin.xyz

TS:   s.indexOf("x")
来源：http://mdy.bbcook.cn

Java: s.indexOf("x")
来源：http://xxk.ivvv.top

Go:   strings.Index(s, "x")
来源：http://uhi.cashguo.top

Ruby: s.index("x")
来源：http://vgf.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://ycz.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jyb.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://obt.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yxt.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aef.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dim.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtn.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://exs.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dco.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kpo.birdmap.top

[E06] 替换子串
来源：http://pxt.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bnm.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://lon.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpf.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://xrt.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqp.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyw.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oyf.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://qlc.zycfv.cn

[E07] 按分隔符拆分
来源：http://dct.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qdh.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avu.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://psh.guannengcc.top

TS:   s.split(",")
来源：http://dhf.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ewe.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vdu.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://dex.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://trq.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://nge.aizwys.cn

Py:   ",".join(items)
来源：http://kqd.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://dih.pycfn.com

JS:   items.join(",")
来源：http://xti.meibo888.top

TS:   items.join(",")
来源：http://nxu.jiagoushi.top

Java: String.join(",", items)
来源：http://org.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://qik.havefunace.top

Ruby: items.join(",")
来源：http://kfo.birdmap.top

C#:   string.Join(",", items)
来源：http://xrn.snrcjt.cn

[E09] 去除所有空白字符
来源：http://vzo.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwb.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://omn.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://tgx.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://rjn.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://hth.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://efo.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cur.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bjm.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://ukk.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mgu.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://csf.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://ujv.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://yzs.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://wla.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fez.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nrp.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vrj.redwolf501.top

[E11] 反转字符串
来源：http://gvq.yuxming.cn

Py:   s[::-1]
来源：http://vjm.nanxuanxn.top

PHP:  strrev($s);
来源：http://jtc.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://mqe.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://ekg.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jsl.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xsj.xuanzx.com

Ruby: s.reverse
来源：http://kyg.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jmw.yueranfly.top

[E12] 统计某字符出现次数
来源：http://fmg.zdbjq.cn

Py:   s.count("a")
来源：http://pyt.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://jof.cucudq.cn

JS:   s.split("a").length - 1
来源：http://sbo.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://ver.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nsx.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://bmn.tanke756.top

Ruby: s.count("a")
来源：http://dht.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://niu.vqdsnc.cn

[E13] 逐字符遍历
来源：http://wpf.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://nnq.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ubl.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zvg.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dmj.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aha.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ksd.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tbn.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cvl.daria6918.cn

[E14] URL 编码与 Base64
来源：http://avx.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kqd.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://anr.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eie.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ruo.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hqr.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qyc.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvo.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://upx.sweek.top

[E15] HTML 转义 / 反转义
来源：http://dcf.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jwr.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ojb.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lpo.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dwv.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oso.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fno.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rsv.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ncs.fanxiaobao.xyz

[E16] 数字千分位
来源：http://kxp.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://efg.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://vbn.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dde.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jxs.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ipe.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kod.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bhk.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://hmb.fehbvm.com

[E17] 首字母大写
来源：http://wrw.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dzm.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tsn.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ves.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opu.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://veh.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ixf.vqdsnc.cn

Ruby: s.capitalize
来源：http://tks.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wcy.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://shb.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://erk.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bxp.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://axh.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wdv.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dae.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xwi.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zrl.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dbq.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://ijl.cashguo.top

Py:   s.splitlines()
来源：http://yya.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://plx.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://wxh.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://qhk.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://rgv.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://gmi.xuetiantiany.cn

Ruby: s.lines
来源：http://aut.sysykeji.top

C#:   s.Split('\n')
来源：http://dai.hnqzz.top

[E20] 判断字符串是否为空
来源：http://kwl.fktsv.cn

Py:   if not s:
来源：http://zdj.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qcx.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://for.zhijiandao.cn

TS:   if (s === "") {}
来源：http://qsh.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://uyz.epnwcf.com

Go:   if s == "" {}
来源：http://jxe.birdmap.top

Ruby: if s.empty?
来源：http://rwy.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pkx.tianlin.xyz

[E21] 超长截断加省略号
来源：http://kbu.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xgu.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yzm.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdw.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmf.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ecp.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://pzj.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pfs.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gdd.xuanzx.com

[E22] 字节长度与字符长度
来源：http://sxf.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fwp.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyi.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibx.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqa.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cnw.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cda.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://huc.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqb.hnqzz.top

================================================================================
来源：http://yhv.shuidangran.top

F. 文件与目录
来源：http://dzt.svipenyu.cn

================================================================================
来源：http://mfg.hcnkem.com

[F01] 读取整个文件
来源：http://ypa.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uzw.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://dcl.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rqi.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dls.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fvf.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eoh.yonumen.top

Ruby: File.read("a.txt")
来源：http://hcj.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://hxw.quarkkingdee.top

[F02] 逐行读取文件
来源：http://dzw.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cse.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://phr.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rdf.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgw.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ccx.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yxj.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zmn.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lvb.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://bdm.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xwy.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sjl.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://koa.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ltb.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ict.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vfl.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://oca.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fpu.smart0.xyz

[F04] 追加写入文件
来源：http://lwu.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nll.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xlt.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lcn.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iih.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yxn.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zze.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wiy.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxu.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://ksd.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kex.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://phr.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://hqo.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://efh.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jgk.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vxa.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://nqw.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://wdi.cdnleiting.top

[F06] 删除文件
来源：http://zgl.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://ozl.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://sxk.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://afl.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://cis.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://azr.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://uxb.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://cbg.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://ffz.fktsv.cn

[F07] 创建目录（含多级）
来源：http://egu.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://asw.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ndw.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aqp.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzs.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rsc.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uun.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gfe.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ltz.hywenlv.cn

[F08] 遍历目录
来源：http://dgi.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ckv.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fey.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://stf.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://yqy.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://usd.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rcf.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://pqs.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://awf.smart0.xyz

[F09] 获取文件大小
来源：http://ewq.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://rlh.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://yyt.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://vky.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://bsz.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://pzo.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwj.jianghu66.top

Ruby: File.size("a.txt")
来源：http://plq.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://coq.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://uej.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xlm.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fdw.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wcy.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://dhu.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xnb.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://obv.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jlx.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://usa.52xcode.cn

[F11] 复制与移动文件
来源：http://pdb.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jmm.fehbvm.com


<!-- 参考信息 -->