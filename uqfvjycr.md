代发 wailian999

PHP:  strpos($s, "x");
来源：http://hns.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nsw.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://juu.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://aux.cheryme.top

Go:   strings.Index(s, "x")
来源：http://obt.0kj1m.cn

Ruby: s.index("x")
来源：http://koo.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://rjp.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nag.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sgf.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://unf.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ozh.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://txa.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mdx.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pda.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nua.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ucl.ctjpmb.com

[E06] 替换子串
来源：http://cwa.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pul.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://pji.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpk.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://oyf.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odo.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ylg.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hsp.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://nxq.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://jzz.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://idn.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywn.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qxk.nwbrower.top

TS:   s.split(",")
来源：http://aah.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kkm.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kxc.cheryme.top

Ruby: s.split(",");  s.split
来源：http://rgo.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ldt.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://aji.pengpengdd.cyou

Py:   ",".join(items)
来源：http://sub.ivvv.top

PHP:  implode(",", $items);
来源：http://gwb.xziqi.cn

JS:   items.join(",")
来源：http://zzl.ydjk.org.cn

TS:   items.join(",")
来源：http://gpp.feifeiyinyue.top

Java: String.join(",", items)
来源：http://uhj.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://ccb.xuanzx.com

Ruby: items.join(",")
来源：http://djo.zycfv.cn

C#:   string.Join(",", items)
来源：http://zcb.pycfn.com

[E09] 去除所有空白字符
来源：http://wdp.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eox.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://phj.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://xcs.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://mkx.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://sic.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zqz.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://ddf.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggc.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://xlm.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rzs.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cdx.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://roc.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://wis.yongpay.top

Java: String.format("%03d", 7)
来源：http://ote.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bje.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gxc.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzy.gotoacloud.top

[E11] 反转字符串
来源：http://qjg.52xcode.cn

Py:   s[::-1]
来源：http://gfs.wangshuangyany.cn

PHP:  strrev($s);
来源：http://cji.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://jaj.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://gxp.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ipz.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://asq.ehwqpu.com

Ruby: s.reverse
来源：http://ird.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ftr.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://jgd.zhiwuduotai.top

Py:   s.count("a")
来源：http://scn.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://glu.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://nov.fktsv.cn

TS:   s.split("a").length - 1
来源：http://bcq.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uiz.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://eid.daxiang520.top

Ruby: s.count("a")
来源：http://bcu.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://mnh.gogol.net.cn

[E13] 逐字符遍历
来源：http://zim.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://yii.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lmp.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hqd.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lao.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://erk.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yrq.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://uxt.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mwu.vehdjk.com

[E14] URL 编码与 Base64
来源：http://jud.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://osw.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vfa.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gok.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://umv.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xpq.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uda.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nck.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tza.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://org.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dmy.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nyp.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://czc.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lue.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://igp.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ycg.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lro.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://syy.zdqjudy.top

[E16] 数字千分位
来源：http://fsc.gzhubu.top

Py:   f"{1234567:,}"
来源：http://ody.yuxming.cn

PHP:  number_format(1234567);
来源：http://jrp.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://oqn.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oau.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vao.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://avd.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kac.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://fwr.zhijiandao.cn

[E17] 首字母大写
来源：http://xan.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://evg.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fmm.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iun.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vqc.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dpg.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ove.yvedp.cn

Ruby: s.capitalize
来源：http://qte.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pju.iojbl.cn

[E18] 模板占位符替换
来源：http://ork.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eem.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fyr.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sfl.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vgm.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gcd.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iak.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gfd.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kee.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://sse.hnqzz.top

Py:   s.splitlines()
来源：http://wlt.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://frj.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://rad.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://iln.jqgfzy.top

Java: s.lines().toList()
来源：http://yds.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://bcx.jinghuilouyu.cn

Ruby: s.lines
来源：http://eci.nwbrower.top

C#:   s.Split('\n')
来源：http://dij.bjfxy.top

[E20] 判断字符串是否为空
来源：http://rvg.hesvh.cn

Py:   if not s:
来源：http://fqt.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyg.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ekn.yanxiufei.cn

TS:   if (s === "") {}
来源：http://uyx.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://xpf.zhijiandao.cn

Go:   if s == "" {}
来源：http://bea.bbcook.cn

Ruby: if s.empty?
来源：http://oxa.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://amu.cheryme.top

[E21] 超长截断加省略号
来源：http://smh.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zkn.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ysj.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsc.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbk.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahl.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://elb.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ndx.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ylq.havefunace.top

[E22] 字节长度与字符长度
来源：http://fxn.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mye.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gxl.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hvf.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://slx.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzl.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hmd.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://ogj.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kwb.tarul.cn

================================================================================
来源：http://yin.gzhubu.top

F. 文件与目录
来源：http://vkm.fktsv.cn

================================================================================
来源：http://qvr.jinqigufen.top

[F01] 读取整个文件
来源：http://cxh.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://upb.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://yre.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bny.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpe.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qij.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rzx.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://ssh.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://gnb.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://obz.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hkb.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qul.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mqc.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oxj.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://moa.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vhi.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azp.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgf.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://chu.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yvc.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nmm.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvl.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ccm.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://epc.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jme.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://jop.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://czj.yonumen.top

[F04] 追加写入文件
来源：http://ccn.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ukr.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://emn.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://llc.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzq.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uks.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhr.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vff.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cug.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://ngr.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzy.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://heo.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://pms.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://iew.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zoj.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qvf.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://qrn.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://bxq.chenjidiqi.icu

[F06] 删除文件
来源：http://nrc.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://mdy.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://ewy.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://pre.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://arz.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rnr.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://yqd.hammf.cn

Ruby: File.delete("a.txt")
来源：http://jwm.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://yvf.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://bar.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rkw.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wkc.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eto.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cad.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hcx.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dtf.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pwe.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oxj.xuanzx.com

[F08] 遍历目录
来源：http://gja.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ytd.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://smg.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://rro.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://zur.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nwb.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pml.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://edl.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://bcl.shuidangran.top

[F09] 获取文件大小
来源：http://ezn.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://kzu.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://wrk.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://ovr.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://bcg.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://ozt.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://isc.cucudq.cn

Ruby: File.size("a.txt")
来源：http://esq.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://nme.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://usg.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://prr.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cli.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bex.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://fik.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://agt.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://beq.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gfv.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yvd.cheryme.top

[F11] 复制与移动文件
来源：http://hib.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hyi.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fjf.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zox.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fif.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ooq.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nqf.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipc.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vqz.shangyingyoupin.top

[F12] CSV 读写
来源：http://ilx.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rdb.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://akd.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iig.yonumen.top

TS:   // 同上
来源：http://uga.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kvy.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lrk.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://isq.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rie.xuanzx.com

================================================================================
来源：http://apx.jinyuanbaomall.cn

G. 面向对象
来源：http://yfk.yongpay.top

================================================================================
来源：http://bxu.shangyingyoupin.top

[G01] 定义类
来源：http://rdp.xuanzx.com

Py:   class User: pass
来源：http://ofi.ybcxt.top

PHP:  class User {}
来源：http://uie.yj202588.top

JS:   class User {}
来源：http://duf.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://gbp.aibaodan.cn

Java: class User {}
来源：http://xsz.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://iby.jinyuanbaomall.cn

Ruby: class User; end
来源：http://tba.iojbl.cn

C#:   class User {}
来源：http://nco.zdbjq.cn

[G02] 构造函数
来源：http://wbm.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://zwj.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://gqh.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://uwb.ivvv.top

TS:   constructor(public name: string) {}
来源：http://krt.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://wsv.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iml.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://knd.kuanghao11.cn


<!-- 参考信息 -->