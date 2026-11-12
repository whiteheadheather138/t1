代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hjq.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lux.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rxh.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://hnl.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uca.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sbi.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zst.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dzx.yuanzhike.top

[E06] 替换子串
来源：http://itc.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hkj.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://uvd.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sqm.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://jbo.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpw.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uak.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mwi.316326.xyz

C#:   s.Replace("a", "b")
来源：http://mez.yj20258888.top

[E07] 按分隔符拆分
来源：http://blt.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hvf.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://onv.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://grs.smart0.xyz

TS:   s.split(",")
来源：http://ueh.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://mrn.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oqh.hammf.cn

Ruby: s.split(",");  s.split
来源：http://ham.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nmv.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://wqo.wangdashe.top

Py:   ",".join(items)
来源：http://qsz.zhixingplan.top

PHP:  implode(",", $items);
来源：http://qpo.havefunace.top

JS:   items.join(",")
来源：http://fbt.jinqigufen.top

TS:   items.join(",")
来源：http://dsd.xinyue.icu

Java: String.join(",", items)
来源：http://jwc.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://rwi.yj20258.top

Ruby: items.join(",")
来源：http://raa.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://qqi.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://fwt.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nti.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wps.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://bft.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://nol.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://pgc.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uas.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://xxw.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qap.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://trq.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blr.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cog.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://prt.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://cmi.fehbvm.com

Java: String.format("%03d", 7)
来源：http://afk.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rfa.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hvd.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wdc.yj202588.top

[E11] 反转字符串
来源：http://kib.fanxiaobao.xyz

Py:   s[::-1]
来源：http://bxh.quarkkingdee.top

PHP:  strrev($s);
来源：http://pne.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://lby.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://mrm.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://flk.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://cth.chenlongwang.top

Ruby: s.reverse
来源：http://cmm.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lzp.xziqi.cn

[E12] 统计某字符出现次数
来源：http://wep.fzhhl.top

Py:   s.count("a")
来源：http://sbs.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://kpv.wangdashe.top

JS:   s.split("a").length - 1
来源：http://rpa.sweek.top

TS:   s.split("a").length - 1
来源：http://iop.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qls.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://emy.fktsv.cn

Ruby: s.count("a")
来源：http://ffz.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://tvu.aibaodan.cn

[E13] 逐字符遍历
来源：http://fhl.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://nid.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cma.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ama.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qfa.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iap.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qmb.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://elp.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vgw.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://elb.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vdk.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cyw.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gbj.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pys.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tsn.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xvp.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://btw.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ixp.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://tiy.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ftw.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yby.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ruc.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rqa.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zwu.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ove.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ahi.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kjs.meibo888.top

[E16] 数字千分位
来源：http://dpp.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://ntk.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://vcz.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yrb.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://rtf.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qcp.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mve.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qkg.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://mmk.hammf.cn

[E17] 首字母大写
来源：http://rer.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hux.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bbz.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zks.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rka.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mjs.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ijc.xuetiantiany.cn

Ruby: s.capitalize
来源：http://gsh.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://buv.dashuyun.cn

[E18] 模板占位符替换
来源：http://vue.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yex.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dkj.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yfu.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://owt.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://phs.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tiz.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ozo.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nvf.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://zvc.cqqwz.cn

Py:   s.splitlines()
来源：http://urw.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gkd.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://bzl.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://bup.jinqigfzy.top

Java: s.lines().toList()
来源：http://azk.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://ncj.zhengqikj.top

Ruby: s.lines
来源：http://krv.sufxvd.cn

C#:   s.Split('\n')
来源：http://mgf.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://jeu.fehbvm.com

Py:   if not s:
来源：http://mte.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpo.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.jlsjyb.cn

TS:   if (s === "") {}
来源：http://sbw.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://zms.jinqigfzy.top

Go:   if s == "" {}
来源：http://ncu.fengsongda.top

Ruby: if s.empty?
来源：http://dab.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xam.wangdashe.top

[E21] 超长截断加省略号
来源：http://xrz.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fhs.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cuz.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xrp.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbt.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xwy.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://nyt.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rgg.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rsc.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://pfh.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kmc.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsn.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xlc.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvt.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uet.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rfo.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://qfc.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vyz.sjlbkw.cn

================================================================================
来源：http://eut.snrcjt.cn

F. 文件与目录
来源：http://kab.nwbrower.top

================================================================================
来源：http://ncg.yanxiufei.cn

[F01] 读取整个文件
来源：http://fdo.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pwb.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://gvq.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ozh.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ofw.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://oui.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cij.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://qsj.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://kht.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://rer.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://roh.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yka.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxv.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbg.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://icy.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yvw.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jce.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hwo.ivvv.top

[F03] 写入文件（覆盖）
来源：http://fgh.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bve.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://voq.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbi.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ail.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zqn.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tgh.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://ytg.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gzy.jinqigfzy.top

[F04] 追加写入文件
来源：http://esu.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dbp.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kmv.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://scs.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://inu.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wer.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ins.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zcx.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nhw.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://sqe.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gdn.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://zcl.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://elg.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://jxp.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://obo.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wwe.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://eeu.sweek.top

C#:   File.Exists("a.txt")
来源：http://fkj.daxiang520.top

[F06] 删除文件
来源：http://ncm.bjfxy.top

Py:   os.remove("a.txt")
来源：http://vqz.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ldn.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://fes.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dng.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xlo.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://bkv.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://jdh.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://kpw.cashguo.top

[F07] 创建目录（含多级）
来源：http://vri.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cdz.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://egf.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgw.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yng.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mto.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qxm.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sfs.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ubo.zycfv.cn

[F08] 遍历目录
来源：http://ltu.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hrw.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://whk.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://slj.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://oei.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oiq.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hgc.fengsongda.top

Ruby: Dir.children("dir")
来源：http://xxo.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://nig.hywenlv.cn

[F09] 获取文件大小
来源：http://lcf.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://teu.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://sjp.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://dhv.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://zbj.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uzx.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zit.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://hwp.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://zau.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://hca.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eag.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rda.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://doh.ybcxt.top

TS:   path.extname("a.txt")
来源：http://ptk.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dur.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wyb.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cxs.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jcx.yj20258.top

[F11] 复制与移动文件
来源：http://fti.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gbv.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gmq.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tpc.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://znl.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ayo.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://weo.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tux.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xlj.jqgufenzy.top

[F12] CSV 读写
来源：http://fix.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tok.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wau.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eig.hongshengwenyu.top

TS:   // 同上
来源：http://ijr.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ajp.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bku.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lha.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wiy.yangfankeji.com

================================================================================
来源：http://cjo.gogol.net.cn

G. 面向对象
来源：http://ntj.zdqjudy.top

================================================================================
来源：http://psu.yuanzhike.top

[G01] 定义类
来源：http://ndf.c1oappe.top

Py:   class User: pass
来源：http://qqb.cheryme.top

PHP:  class User {}
来源：http://tqq.redwolf501.top

JS:   class User {}
来源：http://qtt.yonumen.top

TS:   class User { name: string = ""; }
来源：http://jdn.andypj.xyz

Java: class User {}
来源：http://jcu.uphjek.com

Go:   type User struct { Name string }
来源：http://mbs.hywenlv.cn

Ruby: class User; end
来源：http://tfr.shangyingyoupin.top

C#:   class User {}
来源：http://vot.jinqigfzy.top

[G02] 构造函数
来源：http://rpw.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://wev.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://khr.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://vuz.tarul.cn

TS:   constructor(public name: string) {}
来源：http://yfk.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://dns.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uwx.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ria.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://wbh.guowangkeji.top

[G03] 实例属性
来源：http://hqu.fengsongda.top

Py:   self.name = "x"
来源：http://boh.yfazqb.com

PHP:  public string $name = "x";
来源：http://bta.jqgufenzy.top

JS:   this.name = "x";
来源：http://uec.jlsjyb.cn

TS:   name: string = "x";
来源：http://dlq.fzhhl.top

Java: private String name;
来源：http://spe.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jok.hongshengwenyu.top


<!-- 参考信息 -->