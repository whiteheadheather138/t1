代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dkj.jyoumei.cn

TS:   s.slice(1, 4)
来源：http://xyh.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://ceg.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uoj.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://etk.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://zkm.jinqigfzy.top

[E04] 查找子串位置
来源：http://hej.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://opi.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://cpn.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ugi.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://cqa.andypj.xyz

Java: s.indexOf("x")
来源：http://elg.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://zle.hesvh.cn

Ruby: s.index("x")
来源：http://mkf.hesvh.cn

C#:   s.IndexOf("x")
来源：http://rnb.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://njn.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://azp.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dyl.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxp.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://alb.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oas.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://heo.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ywe.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mdo.snrcjt.cn

[E06] 替换子串
来源：http://izq.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://msm.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://cyc.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjp.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://hua.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pep.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wes.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xuq.316326.xyz

C#:   s.Replace("a", "b")
来源：http://ysg.daxiang520.top

[E07] 按分隔符拆分
来源：http://hrf.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sgp.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bkd.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwt.gogol.net.cn

TS:   s.split(",")
来源：http://rkt.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://iio.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zog.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://vnz.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fcz.iojbl.cn

[E08] 数组按分隔符合并
来源：http://ejc.yuanzhike.top

Py:   ",".join(items)
来源：http://rke.jinqigufen.top

PHP:  implode(",", $items);
来源：http://edu.hcnkem.com

JS:   items.join(",")
来源：http://kqt.gotoacloud.top

TS:   items.join(",")
来源：http://lik.xylfe.cn

Java: String.join(",", items)
来源：http://xuy.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://plu.hammf.cn

Ruby: items.join(",")
来源：http://khx.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://hda.haohaochexian.top

[E09] 去除所有空白字符
来源：http://nro.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ktk.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://udh.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://emb.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://tpl.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://vge.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmt.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pav.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kvi.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://raz.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gyt.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tcy.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://peq.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://mgh.andypj.xyz

Java: String.format("%03d", 7)
来源：http://ycs.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qtu.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cvq.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gxr.cucudq.cn

[E11] 反转字符串
来源：http://zaq.xinyue.icu

Py:   s[::-1]
来源：http://pnw.0kj1m.cn

PHP:  strrev($s);
来源：http://lhr.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://bjs.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://fnn.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ynn.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lbg.jqgufenzy.top

Ruby: s.reverse
来源：http://frs.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zhk.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://hxo.zhengqikj.top

Py:   s.count("a")
来源：http://bqc.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://pcz.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://ark.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://fvx.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pje.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://ybk.gotoacloud.top

Ruby: s.count("a")
来源：http://jrw.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://fvq.iojbl.cn

[E13] 逐字符遍历
来源：http://dor.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://olr.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lqz.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lhg.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://auo.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zcs.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxv.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://msf.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://owt.yj20258.top

[E14] URL 编码与 Base64
来源：http://qtl.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yxs.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xhg.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xfv.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ype.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tpg.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vpk.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dky.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://clg.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://zsj.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://zkd.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ver.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ata.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lgg.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qke.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cud.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fup.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mgz.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://ezg.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://zwk.fzhhl.top

PHP:  number_format(1234567);
来源：http://wba.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aok.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lab.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ulq.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zfb.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tfl.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://inx.gogol.net.cn

[E17] 首字母大写
来源：http://mlt.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jkp.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyd.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uvf.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fui.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wum.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xse.zhengqikj.top

Ruby: s.capitalize
来源：http://jge.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dhc.hammf.cn

[E18] 模板占位符替换
来源：http://bqs.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lan.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eju.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uie.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iwu.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zpn.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkj.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oyl.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://daa.daxiang520.top

[E19] 多行文本按行拆分
来源：http://lcp.vqdsnc.cn

Py:   s.splitlines()
来源：http://uln.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bkc.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://bgt.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://iux.pengpengdd.cyou

Java: s.lines().toList()
来源：http://muo.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://fbw.sufxvd.cn

Ruby: s.lines
来源：http://hkv.yuxming.cn

C#:   s.Split('\n')
来源：http://zcq.sweek.top

[E20] 判断字符串是否为空
来源：http://pml.yuxming.cn

Py:   if not s:
来源：http://cuw.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zfn.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rpw.cashguo.top

TS:   if (s === "") {}
来源：http://dzn.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://bvm.pycfn.com

Go:   if s == "" {}
来源：http://mkn.quarkkingdee.top

Ruby: if s.empty?
来源：http://wuf.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zgx.0kj1m.cn

[E21] 超长截断加省略号
来源：http://pka.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gzs.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zyx.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zzl.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axp.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://otg.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://dbd.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nwp.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pnu.hcnkem.com

[E22] 字节长度与字符长度
来源：http://wwc.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lpz.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cmw.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mge.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mtw.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gpj.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ons.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://emb.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://olf.sweek.top

================================================================================
来源：http://lbn.kuanghao11.cn

F. 文件与目录
来源：http://awp.yongpay.top

================================================================================
来源：http://ktn.sweek.top

[F01] 读取整个文件
来源：http://ohd.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lta.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://avb.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oit.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uon.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://erj.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kvd.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://vfl.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://zbk.xziqi.cn

[F02] 逐行读取文件
来源：http://ntm.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xuz.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rml.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxg.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://auf.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axu.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://die.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iqu.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wyv.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://qvh.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yrd.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://thh.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbn.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gxo.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kgh.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qsw.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://iho.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://klt.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://com.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://khs.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ltx.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izv.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmv.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gdh.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dbs.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nuu.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sgb.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://ens.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hzy.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://ycv.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://moz.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://ihu.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://alv.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kln.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://xir.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://jig.zdbjq.cn

[F06] 删除文件
来源：http://wvc.xuanzx.com

Py:   os.remove("a.txt")
来源：http://yqb.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://myv.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hxg.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://wpj.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://enr.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://pjd.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://trw.hammf.cn

C#:   File.Delete("a.txt");
来源：http://lrd.sweek.top

[F07] 创建目录（含多级）
来源：http://afl.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iav.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jek.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbd.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrc.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rci.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aat.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gjp.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://quh.fehbvm.com

[F08] 遍历目录
来源：http://qpi.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hev.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://esd.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://sxm.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://xhd.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvm.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xin.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://oqz.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://gzi.daria6918.cn

[F09] 获取文件大小
来源：http://cbl.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://vgz.xziqi.cn

PHP:  filesize("a.txt");
来源：http://nqz.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://vjp.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://oja.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://vjc.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xxt.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://yqp.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://djg.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://hxb.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bdm.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xja.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kes.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://upz.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lio.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sol.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://phq.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nbq.redwolf501.top

[F11] 复制与移动文件
来源：http://fis.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nxa.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bfq.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jww.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kvx.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lkh.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ugs.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqg.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fmw.mhx1999.top

[F12] CSV 读写
来源：http://maa.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jro.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cos.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wjt.yj202588.top

TS:   // 同上
来源：http://wno.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mpq.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mua.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lvu.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hrr.bjfxy.top

================================================================================
来源：http://zhj.dianchejie.cn

G. 面向对象
来源：http://daw.xuanzx.com

================================================================================
来源：http://ulx.yongpay.top

[G01] 定义类
来源：http://sxj.ydzc1.top

Py:   class User: pass
来源：http://nqr.quarkkingdee.top

PHP:  class User {}
来源：http://qku.nanxinkj.top

JS:   class User {}
来源：http://fou.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://hep.hfpthk.cn

Java: class User {}
来源：http://usv.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://jdc.xinyue.icu

Ruby: class User; end
来源：http://vkw.sjlbkw.cn

C#:   class User {}
来源：http://gdf.gotoacloud.top


<!-- 参考信息 -->