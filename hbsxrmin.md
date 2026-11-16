代发 wailian999

================================================================================
来源：http://kqo.yvedp.cn

E. 字符串处理
来源：http://kcb.mhx1999.top

================================================================================
来源：http://tpq.hesvh.cn

[E01] 拼接字符串
来源：http://fcj.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nzj.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ynw.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vqf.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dju.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qxf.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qtw.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kgs.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ohc.yonumen.top

[E02] 重复字符串
来源：http://pug.fehbvm.com

Py:   "ab" * 3
来源：http://pmu.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://tmn.zycfv.cn

JS:   "ab".repeat(3)
来源：http://qel.xinyue.icu

TS:   "ab".repeat(3)
来源：http://fhh.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://oll.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://lbg.c1oappe.top

Ruby: "ab" * 3
来源：http://xdk.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dlw.jinyuanbaomall.cn

[E03] 截取子串
来源：http://dqx.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ouk.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pzw.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bvm.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://jcu.hysaishi.cn

Java: s.substring(1, 4)
来源：http://gok.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ove.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://hmu.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://izq.uphjek.com

[E04] 查找子串位置
来源：http://twu.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://hjz.mhx1999.top

PHP:  strpos($s, "x");
来源：http://nid.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://llu.redwolf501.top

TS:   s.indexOf("x")
来源：http://bis.hcnkem.com

Java: s.indexOf("x")
来源：http://dnu.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://eoe.hammf.cn

Ruby: s.index("x")
来源：http://kfw.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://snl.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://btl.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oqq.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yka.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iow.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://duo.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kql.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wut.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://azz.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kxt.bjfxy.top

[E06] 替换子串
来源：http://zeb.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gpw.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://hpk.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aii.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://qzw.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oow.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mzk.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fgb.meibo888.top

C#:   s.Replace("a", "b")
来源：http://jel.cheryme.top

[E07] 按分隔符拆分
来源：http://ssf.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://awf.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tfh.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tqu.wangdashe.top

TS:   s.split(",")
来源：http://iri.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://egw.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gqr.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://vxk.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eya.yj20258.top

[E08] 数组按分隔符合并
来源：http://psh.quarkkingdee.top

Py:   ",".join(items)
来源：http://zwk.ppjwa.cn

PHP:  implode(",", $items);
来源：http://roi.jinqigfzy.top

JS:   items.join(",")
来源：http://jqh.kuanghao11.cn

TS:   items.join(",")
来源：http://crn.mhx1999.top

Java: String.join(",", items)
来源：http://wtu.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://kgf.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://ifs.xylfe.cn

C#:   string.Join(",", items)
来源：http://qnp.andypj.xyz

[E09] 去除所有空白字符
来源：http://hdf.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pry.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://img.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://zfj.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://sfr.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://qrr.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zzx.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://zak.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://win.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://dpe.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rbo.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vof.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://jdh.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://hcc.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://qbc.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vmk.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xsc.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://utt.hnxiangtu.top

[E11] 反转字符串
来源：http://xpa.ehwqpu.com

Py:   s[::-1]
来源：http://vgw.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://jfu.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://wze.sweek.top

TS:   [...s].reverse().join("")
来源：http://yhx.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hyo.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lst.uphjek.com

Ruby: s.reverse
来源：http://gsh.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uzu.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://ulw.dashuyun.cn

Py:   s.count("a")
来源：http://cvv.ivvv.top

PHP:  substr_count($s, "a");
来源：http://rpt.vehdjk.com

JS:   s.split("a").length - 1
来源：http://vgo.wangdashe.top

TS:   s.split("a").length - 1
来源：http://fls.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vrn.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://uze.hysaishi.cn

Ruby: s.count("a")
来源：http://lbm.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://xro.chenzaomai.com

[E13] 逐字符遍历
来源：http://jvk.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://wyn.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bry.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lpy.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bxk.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edp.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nqn.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rip.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ycm.fengsongda.top

[E14] URL 编码与 Base64
来源：http://jrb.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xlz.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://vih.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ocr.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uil.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ovl.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vwd.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nvp.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfv.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://mhi.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xhd.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gkn.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ocw.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fzc.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rsf.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xro.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jfq.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://djo.zhengqikj.top

[E16] 数字千分位
来源：http://dmo.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://xqr.tianlin.xyz

PHP:  number_format(1234567);
来源：http://qkf.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zox.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ymz.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bbm.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ykm.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mjv.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://zit.52xcode.cn

[E17] 首字母大写
来源：http://usu.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lfx.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://psw.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dcv.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uwu.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dnr.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jbg.yvedp.cn

Ruby: s.capitalize
来源：http://kjo.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://djj.ehwqpu.com

[E18] 模板占位符替换
来源：http://eou.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dcv.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wzg.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jjv.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uoi.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wqq.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://twd.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ggf.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kxi.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://nii.hywenlv.cn

Py:   s.splitlines()
来源：http://zru.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jtz.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://bwl.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://gyw.hnqzz.top

Java: s.lines().toList()
来源：http://dst.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://pam.316326.xyz

Ruby: s.lines
来源：http://ooa.birdmap.top

C#:   s.Split('\n')
来源：http://gta.andypj.xyz

[E20] 判断字符串是否为空
来源：http://jtf.meibo888.top

Py:   if not s:
来源：http://xwp.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oln.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kmv.ctjpmb.com

TS:   if (s === "") {}
来源：http://nvi.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://tdt.bjfxy.top

Go:   if s == "" {}
来源：http://wxd.jqgufenzy.top

Ruby: if s.empty?
来源：http://hgq.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qit.fktsv.cn

[E21] 超长截断加省略号
来源：http://hmq.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ncq.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://htg.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xev.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://txo.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lew.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://llz.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vqz.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://noe.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://hkl.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ubd.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zzu.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qul.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qhg.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bcg.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fmh.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://ckz.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zlq.hywenlv.cn

================================================================================
来源：http://brs.gaohongyu789.top

F. 文件与目录
来源：http://zof.hammf.cn

================================================================================
来源：http://aag.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://fdz.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xgv.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://fzy.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gsa.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://chs.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ytn.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dzx.sweek.top

Ruby: File.read("a.txt")
来源：http://mfe.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://cnr.havefunace.top

[F02] 逐行读取文件
来源：http://emq.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gyd.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rpf.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrk.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fcm.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://srl.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pgl.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://omf.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ect.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://hek.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pbt.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ldq.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xad.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iiv.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bwy.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dxg.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qoq.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bbc.xuetiantiany.cn

[F04] 追加写入文件
来源：http://lry.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ksj.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ite.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vfq.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlv.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://szi.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ckm.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mqi.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hgt.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://syn.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://npa.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://bwv.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://cxc.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://ofy.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mao.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qkh.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://lwf.tarul.cn

C#:   File.Exists("a.txt")
来源：http://het.jinqigufen.top

[F06] 删除文件
来源：http://lhz.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://rdn.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://dti.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yhf.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://qln.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sjp.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://fiz.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://dim.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://crr.fengsongda.top

[F07] 创建目录（含多级）
来源：http://lgh.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xmn.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzb.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psf.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://syu.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osn.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bar.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dpu.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmo.cashguo.top

[F08] 遍历目录
来源：http://bgr.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vui.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kbp.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://dkt.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://wzt.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xjf.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ynr.yfazqb.com

Ruby: Dir.children("dir")
来源：http://zps.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://fvl.jiagoushi.top

[F09] 获取文件大小
来源：http://vld.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://apj.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://vay.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://hcq.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://gwi.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wxx.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bmx.sysykeji.top

Ruby: File.size("a.txt")
来源：http://eby.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://tiy.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://fdo.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://khe.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dxk.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kkh.daria6918.cn

TS:   path.extname("a.txt")
来源：http://soo.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tnx.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lmh.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tgt.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vos.vqdsnc.cn

[F11] 复制与移动文件
来源：http://fir.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://est.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://var.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://his.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxw.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dji.chenlongwang.top


<!-- 参考信息 -->