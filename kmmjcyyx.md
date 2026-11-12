代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owg.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dwu.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vql.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://evn.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tfl.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mnx.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dnl.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jbc.c1oappe.top

[E02] 重复字符串
来源：http://rkn.pengpengdd.cyou

Py:   "ab" * 3
来源：http://chk.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://dsm.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://jga.jianghu66.top

TS:   "ab".repeat(3)
来源：http://ohc.zhengqikj.top

Java: "ab".repeat(3)
来源：http://ojq.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://cxe.dashuyun.cn

Ruby: "ab" * 3
来源：http://qsc.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://esw.hfpthk.cn

[E03] 截取子串
来源：http://glg.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gyg.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihp.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ziy.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://ufj.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://kla.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yei.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dpj.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://jqx.nanxinkj.top

[E04] 查找子串位置
来源：http://qzb.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://yrk.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://ybo.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gll.hnqzz.top

TS:   s.indexOf("x")
来源：http://sac.svipenyu.cn

Java: s.indexOf("x")
来源：http://qfh.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://lnu.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://tsj.hesvh.cn

C#:   s.IndexOf("x")
来源：http://jlg.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ccs.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qcg.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpc.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ksa.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cat.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lvg.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gay.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://apc.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kdk.ppjwa.cn

[E06] 替换子串
来源：http://ewd.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wqx.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://rnu.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyy.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://wfs.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyr.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://osu.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pgr.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://tsk.meibo888.top

[E07] 按分隔符拆分
来源：http://znd.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ghn.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nri.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wac.yj20258.top

TS:   s.split(",")
来源：http://wzc.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mwq.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uif.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://jtx.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bbd.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://ivk.tarul.cn

Py:   ",".join(items)
来源：http://srm.sweek.top

PHP:  implode(",", $items);
来源：http://gtz.guowangkeji.top

JS:   items.join(",")
来源：http://pxo.ehwqpu.com

TS:   items.join(",")
来源：http://csd.dianchejie.cn

Java: String.join(",", items)
来源：http://vso.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://cde.hongshengwenyu.top

Ruby: items.join(",")
来源：http://cba.jianghu66.top

C#:   string.Join(",", items)
来源：http://hoo.yj20258888.top

[E09] 去除所有空白字符
来源：http://alz.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dsz.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tsi.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://pwo.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ese.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://sin.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdw.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bso.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nfw.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://koi.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vhv.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ztp.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://jfh.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://qyq.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://bsl.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lhp.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ufh.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lhc.jiagoushi.top

[E11] 反转字符串
来源：http://qvz.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://ezk.fengsongda.top

PHP:  strrev($s);
来源：http://dlt.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://jtx.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://umd.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qwy.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qbq.shzxlz.cn

Ruby: s.reverse
来源：http://epb.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ryt.havefunace.top

[E12] 统计某字符出现次数
来源：http://qdj.jiagoushi.top

Py:   s.count("a")
来源：http://xvr.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://csh.fengsongda.top

JS:   s.split("a").length - 1
来源：http://fwi.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://han.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ald.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://auo.tian-w.cn

Ruby: s.count("a")
来源：http://ggy.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://bie.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://ujn.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://sow.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lla.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cjq.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xck.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zky.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yoa.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://izf.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wfu.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://xwk.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvs.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ice.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bsq.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzb.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zda.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdt.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://huw.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zqe.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://lji.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mfa.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vjg.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bvw.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hkz.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vmi.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iiw.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mcb.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sno.zhijiandao.cn

[E16] 数字千分位
来源：http://omp.tarul.cn

Py:   f"{1234567:,}"
来源：http://lba.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://nye.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uqi.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hoe.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ylu.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ogt.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ume.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://kix.dashuyun.cn

[E17] 首字母大写
来源：http://tbd.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfg.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nlj.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://txk.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbv.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wak.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hdf.haohaochexian.top

Ruby: s.capitalize
来源：http://vtg.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rye.shuidangran.top

[E18] 模板占位符替换
来源：http://tdw.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gax.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vjo.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aqu.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://qom.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oui.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dny.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ner.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tfm.cashguo.top

[E19] 多行文本按行拆分
来源：http://vbf.cashguo.top

Py:   s.splitlines()
来源：http://ibq.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wec.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://goo.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://ylf.zycfv.cn

Java: s.lines().toList()
来源：http://wtx.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://cxj.tanke756.top

Ruby: s.lines
来源：http://ihb.sxryk.cn

C#:   s.Split('\n')
来源：http://ugh.yueranfly.top

[E20] 判断字符串是否为空
来源：http://jyp.shanyushiyangkeji.top

Py:   if not s:
来源：http://iug.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nbu.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wra.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://jqt.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://fql.hcnkem.com

Go:   if s == "" {}
来源：http://ups.birdmap.top

Ruby: if s.empty?
来源：http://sai.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hkq.redwolf501.top

[E21] 超长截断加省略号
来源：http://eqh.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://edy.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hbc.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsn.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pim.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dyg.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://ndo.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kfm.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dtw.hammf.cn

[E22] 字节长度与字符长度
来源：http://nmo.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yrc.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://obp.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://evj.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://imq.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tcz.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhw.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ohr.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eft.shangyingyoupin.top

================================================================================
来源：http://dau.zhengqikj.top

F. 文件与目录
来源：http://mac.yuanzhike.top

================================================================================
来源：http://tvu.zhoulong.xyz

[F01] 读取整个文件
来源：http://ezg.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gwy.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://pbb.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://osg.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfn.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wft.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://taj.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://qkx.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://nzn.shzxlz.cn

[F02] 逐行读取文件
来源：http://brt.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jqr.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lrc.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xtt.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nzl.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hum.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fuu.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blr.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzi.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://mkz.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zwr.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jjc.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xxt.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cou.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bur.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pis.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://uxj.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tth.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://bok.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwv.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://idc.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://enn.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpo.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://inp.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gpa.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjz.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mfd.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://nbg.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxg.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://yds.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://rif.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://ymb.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://skh.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gax.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://kcb.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://flo.hesvh.cn

[F06] 删除文件
来源：http://bwp.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://dge.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://yxa.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://hic.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gfp.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lld.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://tys.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://xoc.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://kgw.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://cxg.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pjl.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://llp.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzt.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tuv.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hgp.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pay.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aoh.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ypq.nanxinkj.top

[F08] 遍历目录
来源：http://uvu.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bst.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tuc.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://ueh.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://wvs.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://njq.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pey.c1oappe.top

Ruby: Dir.children("dir")
来源：http://qnh.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://olp.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://lcg.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://pwu.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://jsf.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://tfm.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://uhc.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ivk.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dng.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://gxl.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://zjy.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://ngd.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsu.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qtq.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bzc.yvedp.cn

TS:   path.extname("a.txt")
来源：http://pnd.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hkk.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kbg.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://okz.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjd.snrcjt.cn

[F11] 复制与移动文件
来源：http://vrr.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dzh.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wsx.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvv.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vkm.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ozc.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pzg.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bev.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ruu.zhixingplan.top

[F12] CSV 读写
来源：http://nwb.iojbl.cn


<!-- 参考信息 -->