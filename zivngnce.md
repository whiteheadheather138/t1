代发 wailian999

TS:   "ab".repeat(3)
来源：http://pys.tian-w.cn

Java: "ab".repeat(3)
来源：http://wwf.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://fxj.vehdjk.com

Ruby: "ab" * 3
来源：http://rjn.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://byr.shanyushiyangtech.top

[E03] 截取子串
来源：http://qzr.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://imv.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pfy.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://evj.cheryme.top

TS:   s.slice(1, 4)
来源：http://yig.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://zsq.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ekr.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://ehm.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://bvy.zhixingplan.top

[E04] 查找子串位置
来源：http://oxu.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://pyc.havefunace.top

PHP:  strpos($s, "x");
来源：http://gko.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aoz.aibaodan.cn

TS:   s.indexOf("x")
来源：http://tnu.chenlongwang.top

Java: s.indexOf("x")
来源：http://ksq.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://dqe.zhijiandao.cn

Ruby: s.index("x")
来源：http://jbt.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://brv.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rmp.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xfx.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://txg.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kks.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yjk.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhq.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ttk.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oan.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cgb.vqdsnc.cn

[E06] 替换子串
来源：http://hpr.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kqf.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://xup.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvt.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://dej.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eub.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kwp.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xqv.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://evw.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://dum.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tms.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ayj.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oon.gotoacloud.top

TS:   s.split(",")
来源：http://fbx.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pdd.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lrl.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://axp.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lqs.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://igw.hongshengwenyu.top

Py:   ",".join(items)
来源：http://bik.jiagoushi.top

PHP:  implode(",", $items);
来源：http://jgf.jianghu66.top

JS:   items.join(",")
来源：http://wtj.xziqi.cn

TS:   items.join(",")
来源：http://bxn.svipenyu.cn

Java: String.join(",", items)
来源：http://ark.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://yin.nanxuanxn.top

Ruby: items.join(",")
来源：http://iyw.nanxinkj.top

C#:   string.Join(",", items)
来源：http://gnp.tianlin.xyz

[E09] 去除所有空白字符
来源：http://guk.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cnl.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qrp.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://edn.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://cym.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://bed.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pxl.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://odd.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gpw.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://mfg.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sxv.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fdk.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://odb.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://gej.epnwcf.com

Java: String.format("%03d", 7)
来源：http://tvc.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://brc.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gqb.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rhz.zycfv.cn

[E11] 反转字符串
来源：http://uti.hnxiangtu.top

Py:   s[::-1]
来源：http://pnh.nwbrower.top

PHP:  strrev($s);
来源：http://qbm.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://fwd.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://qla.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://brf.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://phn.aibaodan.cn

Ruby: s.reverse
来源：http://tmt.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://nms.sweek.top

[E12] 统计某字符出现次数
来源：http://yhb.smart0.xyz

Py:   s.count("a")
来源：http://zql.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://pzz.yvedp.cn

JS:   s.split("a").length - 1
来源：http://xlx.hnqzz.top

TS:   s.split("a").length - 1
来源：http://uwv.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zjh.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://wic.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://wgj.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://hik.bjfxy.top

[E13] 逐字符遍历
来源：http://lrk.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://qcb.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noy.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zco.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fjw.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iin.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://huu.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vsf.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lam.ybcxt.top

[E14] URL 编码与 Base64
来源：http://prx.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cgf.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://adk.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rea.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://afb.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wch.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tne.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vpt.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqs.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://uiu.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pjl.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qzp.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oym.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://msx.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bgu.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eyf.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nys.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ghp.pengpengdd.cyou

[E16] 数字千分位
来源：http://dss.daria6918.cn

Py:   f"{1234567:,}"
来源：http://bsx.c1oappe.top

PHP:  number_format(1234567);
来源：http://ajb.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ejc.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://xpr.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://psu.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kwd.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qkl.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://vyr.zhengqikj.top

[E17] 首字母大写
来源：http://obr.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fzn.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uya.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jej.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yem.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bbm.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://inz.yonumen.top

Ruby: s.capitalize
来源：http://zul.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rhq.cashguo.top

[E18] 模板占位符替换
来源：http://zsw.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://unm.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wym.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tqj.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xuy.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gnj.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qvc.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xdj.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vys.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://ukc.fengsongda.top

Py:   s.splitlines()
来源：http://txj.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qnd.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://mtc.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://tfh.ivvv.top

Java: s.lines().toList()
来源：http://bbq.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://afe.ctjpmb.com

Ruby: s.lines
来源：http://gvq.jinqigufen.top

C#:   s.Split('\n')
来源：http://ydh.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://jck.cucudq.cn

Py:   if not s:
来源：http://vck.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pfd.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ccj.daria6918.cn

TS:   if (s === "") {}
来源：http://mpb.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://tvc.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://qvk.yvedp.cn

Ruby: if s.empty?
来源：http://net.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uek.yueranfly.top

[E21] 超长截断加省略号
来源：http://pvs.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mok.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sws.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cnk.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://khh.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uhc.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://cko.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jnp.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kxb.yongpay.top

[E22] 字节长度与字符长度
来源：http://miy.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eyt.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://spt.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwh.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkf.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sgi.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fut.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://gvl.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bln.shanyushiyangtech.top

================================================================================
来源：http://ohm.zhijiandao.cn

F. 文件与目录
来源：http://nii.jlsjyb.cn

================================================================================
来源：http://jwa.xziqi.cn

[F01] 读取整个文件
来源：http://tsv.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://luz.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://mjd.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xps.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dhi.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tny.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://opk.yongpay.top

Ruby: File.read("a.txt")
来源：http://miv.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://ntx.guannengcc.top

[F02] 逐行读取文件
来源：http://rsb.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fzd.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xpp.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rul.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vqd.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://evx.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hwz.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lbt.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fie.ivvv.top

[F03] 写入文件（覆盖）
来源：http://ayw.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ekp.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://koc.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gmu.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpy.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mgq.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://leu.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://nha.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cdg.vqdsnc.cn

[F04] 追加写入文件
来源：http://jiu.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wmz.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://btd.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfo.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzn.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wgr.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cef.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bzm.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cts.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://pmy.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vqc.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://jle.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://xlf.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://tum.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bil.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gkp.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://vsc.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://vpe.ywan-chungtsiang.top

[F06] 删除文件
来源：http://wku.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://kuq.316326.xyz

PHP:  unlink("a.txt");
来源：http://aab.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bxw.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nqn.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yrb.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://hzb.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://wkp.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://wyr.uphjek.com

[F07] 创建目录（含多级）
来源：http://oce.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kaa.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vkf.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xah.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tyo.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iwr.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fyr.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cne.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ndn.yuxming.cn

[F08] 遍历目录
来源：http://qpz.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://npt.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://drc.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://isc.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://vut.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sto.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gdo.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://hzl.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://trc.aizwys.cn

[F09] 获取文件大小
来源：http://npf.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://hzq.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://pba.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://uyd.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://mfo.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://aws.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehu.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://zmk.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://hxk.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://gtw.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gjx.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://djn.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jro.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://ekg.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zwm.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zmh.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ddl.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yak.meibo888.top

[F11] 复制与移动文件
来源：http://tje.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zve.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wun.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onc.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tht.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cav.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://prq.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xhh.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jto.pengpengdd.cyou

[F12] CSV 读写
来源：http://kqs.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ywh.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zol.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ora.zhengqikj.top

TS:   // 同上
来源：http://jhr.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wrd.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gla.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hzm.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lyp.redwolf501.top

================================================================================
来源：http://qkq.chenzaomai.com

G. 面向对象
来源：http://aqy.iojbl.cn

================================================================================
来源：http://zjr.xuanzx.com

[G01] 定义类
来源：http://fye.redwolf501.top


<!-- 参考信息 -->