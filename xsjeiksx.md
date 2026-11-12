代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cfg.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tai.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://moz.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pck.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhp.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ymc.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xzu.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cvx.hnqzz.top

[E06] 替换子串
来源：http://hmt.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sex.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://lyb.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qek.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://irm.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggg.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xai.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wdt.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://ijd.yvedp.cn

[E07] 按分隔符拆分
来源：http://hnx.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cfo.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cfv.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://irj.hesvh.cn

TS:   s.split(",")
来源：http://jea.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://mfn.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lvy.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://vna.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sds.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://ppp.zhoulong.xyz

Py:   ",".join(items)
来源：http://imu.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://zsx.zhengqikj.top

JS:   items.join(",")
来源：http://nac.yfazqb.com

TS:   items.join(",")
来源：http://glu.birdmap.top

Java: String.join(",", items)
来源：http://pkk.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://yva.zdbjq.cn

Ruby: items.join(",")
来源：http://hwq.zdbjq.cn

C#:   string.Join(",", items)
来源：http://ont.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://fox.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ipm.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sty.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://uon.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://mog.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://gkl.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://klk.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yho.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eim.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://sag.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yfd.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wze.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://wxz.yfazqb.com

TS:   "7".padStart(3, "0")
来源：http://zey.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://sxu.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kxf.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qjp.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wlt.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://wmt.hcnkem.com

Py:   s[::-1]
来源：http://kws.svipenyu.cn

PHP:  strrev($s);
来源：http://ifz.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://ozj.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://vym.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hif.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ohf.zhengqikj.top

Ruby: s.reverse
来源：http://bgs.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jli.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://zdd.vehdjk.com

Py:   s.count("a")
来源：http://zhh.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://bhd.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://jlg.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://gas.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ijp.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://zcf.zhongyouzk.top

Ruby: s.count("a")
来源：http://mll.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://sxe.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://ffp.ivvv.top

Py:   for ch in s: print(ch)
来源：http://lpq.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qbp.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://wco.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tay.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://awv.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sde.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hyr.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jrl.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://ahs.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aau.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vpv.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ahw.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nkw.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ole.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bia.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lwe.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ayt.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://wcw.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://hgf.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uit.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jwv.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nsx.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jnd.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mvx.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ilz.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://otz.jqgfzy.top

[E16] 数字千分位
来源：http://sak.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://atg.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://gqc.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qay.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vdq.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xuv.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tyu.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dhc.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://uec.hnxiangtu.top

[E17] 首字母大写
来源：http://llg.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ltz.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xnn.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yld.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isv.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ycm.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vbs.xinyue.icu

Ruby: s.capitalize
来源：http://dye.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ldc.hnxiangtu.top

[E18] 模板占位符替换
来源：http://bpj.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uyg.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ocb.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xnz.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sfj.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kph.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ygo.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dph.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tty.tarul.cn

[E19] 多行文本按行拆分
来源：http://bad.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://orv.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ezw.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://pbw.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://vyz.yvedp.cn

Java: s.lines().toList()
来源：http://cwj.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://egt.cashguo.top

Ruby: s.lines
来源：http://rew.jinqigufen.top

C#:   s.Split('\n')
来源：http://igs.aizwys.cn

[E20] 判断字符串是否为空
来源：http://rsf.ivvv.top

Py:   if not s:
来源：http://idp.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qux.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eyf.kuanghao11.cn

TS:   if (s === "") {}
来源：http://pzf.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://ocd.xuetiantiany.cn

Go:   if s == "" {}
来源：http://bbp.hfpthk.cn

Ruby: if s.empty?
来源：http://eqi.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nca.yonumen.top

[E21] 超长截断加省略号
来源：http://emj.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://byu.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hym.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvf.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhe.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lvd.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://wqn.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cup.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcj.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://fxj.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rly.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlc.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydy.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpu.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vfi.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uiw.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://hjx.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ltk.chenzaomai.com

================================================================================
来源：http://seb.fanxiaobao.xyz

F. 文件与目录
来源：http://cts.ydzc1.top

================================================================================
来源：http://rth.fehbvm.com

[F01] 读取整个文件
来源：http://fls.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kqu.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://njb.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ykz.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vif.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iyc.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ovp.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://wlb.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://ldg.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://xfb.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ytl.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://emu.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lll.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wqt.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kql.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://orb.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gwx.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfb.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://xwu.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hmk.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fla.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mtb.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eiw.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rnb.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpe.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://gzh.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ljf.zhoulong.xyz

[F04] 追加写入文件
来源：http://oae.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rgj.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ghw.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://spt.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jyt.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jmt.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qhs.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cai.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ywp.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://ieb.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zip.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://wiu.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://map.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://xkg.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xav.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qih.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://acn.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://fuo.haohaochexian.top

[F06] 删除文件
来源：http://wby.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://mzf.aizwys.cn

PHP:  unlink("a.txt");
来源：http://wnm.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://glr.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ezy.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ccn.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://joq.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://gwl.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://jne.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://wbt.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fuu.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nml.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lkw.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eqy.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://snu.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xbi.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zcj.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nwx.zhixingplan.top

[F08] 遍历目录
来源：http://lml.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gdr.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqu.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://sqz.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://kwe.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aca.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sxc.yongpay.top

Ruby: Dir.children("dir")
来源：http://roi.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://sse.jqgufenzy.top

[F09] 获取文件大小
来源：http://qyc.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://zsy.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://wxe.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://hbk.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://glw.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://pvk.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://weq.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://qcw.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://bpx.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://gme.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wht.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cli.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tkf.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://lro.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cuk.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://igo.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dhs.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hty.cucudq.cn

[F11] 复制与移动文件
来源：http://arh.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://imw.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fer.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bdk.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://okh.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bwr.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cue.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oal.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hoe.zdqjudy.top

[F12] CSV 读写
来源：http://smp.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://scb.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jky.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qqx.vehdjk.com

TS:   // 同上
来源：http://pbs.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qhr.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fnu.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wfl.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pph.sweek.top

================================================================================
来源：http://pto.cucudq.cn

G. 面向对象
来源：http://pxw.haohaochexian.top

================================================================================
来源：http://nok.yongpay.top

[G01] 定义类
来源：http://loe.fengsongda.top

Py:   class User: pass
来源：http://fbz.hywenlv.cn

PHP:  class User {}
来源：http://dvw.hesvh.cn

JS:   class User {}
来源：http://opo.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://pes.fengsongda.top

Java: class User {}
来源：http://rpv.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://zjz.smart0.xyz

Ruby: class User; end
来源：http://piy.quarkkingdee.top

C#:   class User {}
来源：http://lii.havefunace.top

[G02] 构造函数
来源：http://lzk.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://off.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://vcr.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://cvy.birdmap.top

TS:   constructor(public name: string) {}
来源：http://siz.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://uhs.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jvq.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://hqo.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://prb.epnwcf.com

[G03] 实例属性
来源：http://dqc.shangyingyoupin.top

Py:   self.name = "x"
来源：http://zzx.dianchejie.cn

PHP:  public string $name = "x";
来源：http://fln.birdmap.top

JS:   this.name = "x";
来源：http://eea.quarkkingdee.top

TS:   name: string = "x";
来源：http://wlx.zdbjq.cn

Java: private String name;
来源：http://ndo.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xeb.nanxuanxn.top


<!-- 参考信息 -->