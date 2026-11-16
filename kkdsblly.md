代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqh.tianlin.xyz

[E03] 截取子串
来源：http://wus.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fcb.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jdn.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pry.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://ibr.fengsongda.top

Java: s.substring(1, 4)
来源：http://ghl.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hpz.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://esf.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://cwq.jinqigufen.top

[E04] 查找子串位置
来源：http://dra.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://rjv.cheryme.top

PHP:  strpos($s, "x");
来源：http://rlm.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amb.birdmap.top

TS:   s.indexOf("x")
来源：http://omp.52xcode.cn

Java: s.indexOf("x")
来源：http://mpd.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://twu.aizwys.cn

Ruby: s.index("x")
来源：http://jgc.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://owk.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://obe.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://svr.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mmb.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbh.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jox.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbf.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fan.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ksf.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bhb.316326.xyz

[E06] 替换子串
来源：http://ddc.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yus.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://plv.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mky.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://hcs.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://irq.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qwd.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmm.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://ygs.guannengcc.top

[E07] 按分隔符拆分
来源：http://ypm.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qxv.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nxf.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zeq.havefunace.top

TS:   s.split(",")
来源：http://igm.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://noz.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wtt.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://jpt.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qut.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://cqn.chenjidiqi.icu

Py:   ",".join(items)
来源：http://lgg.ehwqpu.com

PHP:  implode(",", $items);
来源：http://mis.zdbjq.cn

JS:   items.join(",")
来源：http://wel.haohaochexian.top

TS:   items.join(",")
来源：http://hil.ctjpmb.com

Java: String.join(",", items)
来源：http://jdo.yongpay.top

Go:   strings.Join(items, ",")
来源：http://dvn.fzhhl.top

Ruby: items.join(",")
来源：http://fmt.yangfankeji.com

C#:   string.Join(",", items)
来源：http://phh.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://pmz.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yyk.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pzp.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://qil.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://owj.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://qrj.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aha.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eol.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://saz.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://trv.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tfq.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lut.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://rew.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://vaq.tanke756.top

Java: String.format("%03d", 7)
来源：http://zli.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zza.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nes.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dqq.ybcxt.top

[E11] 反转字符串
来源：http://vbx.sufxvd.cn

Py:   s[::-1]
来源：http://bjs.snrcjt.cn

PHP:  strrev($s);
来源：http://sic.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://xbh.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://gqh.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zet.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ycq.pycfn.com

Ruby: s.reverse
来源：http://hzw.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qvp.316326.xyz

[E12] 统计某字符出现次数
来源：http://ypr.cdnleiting.top

Py:   s.count("a")
来源：http://jnd.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://pge.vehdjk.com

JS:   s.split("a").length - 1
来源：http://nxz.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://wuz.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vad.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://oxf.fengsongda.top

Ruby: s.count("a")
来源：http://orw.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://dkb.chenzaomai.com

[E13] 逐字符遍历
来源：http://qbr.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://dyp.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vfw.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://rla.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ult.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zke.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://png.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hih.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mtt.gzhubu.top

[E14] URL 编码与 Base64
来源：http://dpx.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://slm.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lqh.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yeo.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zaf.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gcd.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rzn.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fah.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pyy.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://suw.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zlj.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ief.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rnb.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lhu.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://syc.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://owa.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ifl.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hrg.aibaodan.cn

[E16] 数字千分位
来源：http://bgm.fktsv.cn

Py:   f"{1234567:,}"
来源：http://qnw.gotoacloud.top

PHP:  number_format(1234567);
来源：http://ohf.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ein.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lqg.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ktr.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mer.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://otq.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://cfr.sufxvd.cn

[E17] 首字母大写
来源：http://fet.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oho.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iku.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://syg.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kid.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvu.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qvq.zhijiandao.cn

Ruby: s.capitalize
来源：http://xon.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pps.shuidangran.top

[E18] 模板占位符替换
来源：http://kej.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pxt.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zbc.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ouo.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://czg.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://csc.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ygi.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zuq.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gzr.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://xkz.zhoulong.xyz

Py:   s.splitlines()
来源：http://jfr.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ibq.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://xyn.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://lya.zhiwuduotai.top

Java: s.lines().toList()
来源：http://vld.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://fie.ydjk.org.cn

Ruby: s.lines
来源：http://ynn.birdmap.top

C#:   s.Split('\n')
来源：http://gcg.cucudq.cn

[E20] 判断字符串是否为空
来源：http://xcv.daria6918.cn

Py:   if not s:
来源：http://wkx.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gaw.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jzy.zdbjq.cn

TS:   if (s === "") {}
来源：http://oir.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://etm.vqdsnc.cn

Go:   if s == "" {}
来源：http://znj.zhongyouzk.top

Ruby: if s.empty?
来源：http://zcl.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://joc.ybcxt.top

[E21] 超长截断加省略号
来源：http://asa.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://guh.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sbt.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afw.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gno.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rnn.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://jkr.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://inm.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nhq.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://lrh.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://drh.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://inu.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfn.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nme.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fie.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yzw.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://zcz.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://snr.quarkkingdee.top

================================================================================
来源：http://fll.zycfv.cn

F. 文件与目录
来源：http://ura.shanyushiyangkeji.top

================================================================================
来源：http://krc.dianchejie.cn

[F01] 读取整个文件
来源：http://gnv.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xjo.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://iol.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hbs.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bcc.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eig.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iho.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://vwb.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://yhr.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://vrf.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ybh.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rlj.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdy.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otf.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kgh.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sal.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://che.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wlq.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://qlv.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jjl.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aar.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bmp.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lxq.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bro.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xeo.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://uvq.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mgu.yfazqb.com

[F04] 追加写入文件
来源：http://abt.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jkm.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lpf.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jrk.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eiw.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dyk.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://alt.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rvd.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ahx.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://qgs.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kmy.cheryme.top

PHP:  file_exists("a.txt");
来源：http://gjh.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://fiy.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://vov.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://krr.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qbm.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://nnt.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://dtj.ydzc1.top

[F06] 删除文件
来源：http://nid.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://ldr.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://wvf.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://tlh.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://gnf.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://axg.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://clo.yongpay.top

Ruby: File.delete("a.txt")
来源：http://wms.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://rcu.yueranfly.top

[F07] 创建目录（含多级）
来源：http://exa.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lmg.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cpi.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxs.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbx.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nyl.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mbb.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://srz.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqg.wangshuangyany.cn

[F08] 遍历目录
来源：http://vem.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rsg.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://adw.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://hsn.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://wjt.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rea.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xwv.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://lfu.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://mtn.yj202588.top

[F09] 获取文件大小
来源：http://iac.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://mga.uphjek.com

PHP:  filesize("a.txt");
来源：http://xhk.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://lxz.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://blz.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://omp.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wzo.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://fzo.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://tcd.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://uwp.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dwo.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jql.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eom.xziqi.cn

TS:   path.extname("a.txt")
来源：http://jir.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sap.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rai.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ouc.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ehi.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://yaj.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qnm.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://frp.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ykd.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://toh.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zxr.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wsn.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bey.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kov.hesvh.cn

[F12] CSV 读写
来源：http://yln.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wpb.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iyn.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dym.fehbvm.com

TS:   // 同上
来源：http://ssj.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mcv.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vqv.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvm.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eyc.yonumen.top

================================================================================
来源：http://kmz.hcnkem.com

G. 面向对象
来源：http://bcl.smart0.xyz

================================================================================
来源：http://oxw.hongshengwenyu.top

[G01] 定义类
来源：http://yll.sjlbkw.cn

Py:   class User: pass
来源：http://psj.chenjidiqi.icu

PHP:  class User {}
来源：http://yht.jqgfzy.top

JS:   class User {}
来源：http://eji.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://ydt.shzxlz.cn


<!-- 参考信息 -->