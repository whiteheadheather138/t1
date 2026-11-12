代发 wailian999

Go:   strings.Index(s, "x")
来源：http://kvk.nanxuanxn.top

Ruby: s.index("x")
来源：http://xmf.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://uiv.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://buo.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nhq.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fdf.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wzq.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ael.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnr.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zju.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aoz.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qkn.yueranfly.top

[E06] 替换子串
来源：http://bna.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sbf.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://quq.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sns.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://dbz.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ydi.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ixf.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uqu.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://xqh.hcnkem.com

[E07] 按分隔符拆分
来源：http://nok.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dyd.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cue.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hdq.iojbl.cn

TS:   s.split(",")
来源：http://dcc.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://hkq.cdnleiting.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://laq.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://ljh.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emn.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://apd.ydjk.org.cn

Py:   ",".join(items)
来源：http://zww.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://tex.vqdsnc.cn

JS:   items.join(",")
来源：http://qlm.jianghu66.top

TS:   items.join(",")
来源：http://utx.feifeiyinyue.top

Java: String.join(",", items)
来源：http://dzr.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://znk.dashuyun.cn

Ruby: items.join(",")
来源：http://jkj.svipenyu.cn

C#:   string.Join(",", items)
来源：http://ske.yuanzhike.top

[E09] 去除所有空白字符
来源：http://hui.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uao.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qek.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://gxb.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://rhb.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://uad.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dyw.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://vlv.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zjc.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://ibp.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gjm.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mjo.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://xsc.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://dqd.meibo888.top

Java: String.format("%03d", 7)
来源：http://xcu.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://eaf.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fwu.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywk.gotoacloud.top

[E11] 反转字符串
来源：http://fwm.vqdsnc.cn

Py:   s[::-1]
来源：http://vcd.dashuyun.cn

PHP:  strrev($s);
来源：http://mco.sweek.top

JS:   [...s].reverse().join("")
来源：http://ocz.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://hjf.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uxt.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://vwz.daxiang520.top

Ruby: s.reverse
来源：http://cqa.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://pyh.havefunace.top

[E12] 统计某字符出现次数
来源：http://ggm.dashuyun.cn

Py:   s.count("a")
来源：http://yqe.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://ymj.wangdashe.top

JS:   s.split("a").length - 1
来源：http://ubn.smart0.xyz

TS:   s.split("a").length - 1
来源：http://ipr.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ouf.havefunace.top

Go:   strings.Count(s, "a")
来源：http://zjs.chenzaomai.com

Ruby: s.count("a")
来源：http://ous.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://nun.yvedp.cn

[E13] 逐字符遍历
来源：http://lsh.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://vgn.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://viw.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fuo.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swo.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xkq.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://raq.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jkh.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://won.daxiang520.top

[E14] URL 编码与 Base64
来源：http://whn.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uxa.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dko.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bab.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dkw.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wkl.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ccp.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fzn.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nas.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://ctf.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sgy.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvx.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fbm.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://tpr.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jef.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hio.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cws.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nqk.jianghu66.top

[E16] 数字千分位
来源：http://vyv.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://qyu.gotoacloud.top

PHP:  number_format(1234567);
来源：http://ege.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pwn.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wks.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://efv.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hao.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gbb.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://dxc.hnqzz.top

[E17] 首字母大写
来源：http://bas.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gfp.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fhp.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nnz.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzi.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rfn.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dip.birdmap.top

Ruby: s.capitalize
来源：http://iev.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ftc.sjlbkw.cn

[E18] 模板占位符替换
来源：http://jpo.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ciy.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uby.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jnc.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://msq.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kae.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lly.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nqj.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qmb.gzhubu.top

[E19] 多行文本按行拆分
来源：http://rof.xinyue.icu

Py:   s.splitlines()
来源：http://uaj.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyz.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://bst.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://pkn.chenjidiqi.icu

Java: s.lines().toList()
来源：http://ldi.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://mkf.cdnleiting.top

Ruby: s.lines
来源：http://puw.aizwys.cn

C#:   s.Split('\n')
来源：http://ytj.daria6918.cn

[E20] 判断字符串是否为空
来源：http://khc.aizwys.cn

Py:   if not s:
来源：http://jpm.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yqk.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yba.yfazqb.com

TS:   if (s === "") {}
来源：http://gkc.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://jnr.gaohongyu789.top

Go:   if s == "" {}
来源：http://edm.sufxvd.cn

Ruby: if s.empty?
来源：http://teb.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xwj.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://kdb.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yzy.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ztl.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tch.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sls.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ksk.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://kim.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rho.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ubs.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://lqv.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wlb.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xmr.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbt.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyq.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hql.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jjr.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://zsv.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yee.gaohongyu789.top

================================================================================
来源：http://juc.tianlin.xyz

F. 文件与目录
来源：http://hwh.pycfn.com

================================================================================
来源：http://myk.epnwcf.com

[F01] 读取整个文件
来源：http://duj.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://apl.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://frc.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rpl.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uji.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yxf.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://flk.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://znn.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yhd.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://ybm.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qla.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ltb.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xix.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zem.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hqz.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dcq.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ofd.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uuo.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://tqh.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lif.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dwv.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cgl.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pdy.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qhp.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://odc.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://kgm.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dsr.jlsjyb.cn

[F04] 追加写入文件
来源：http://mtz.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ccc.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xwo.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxv.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wkh.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gsc.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jan.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://irf.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iac.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://slc.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pjg.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://dbg.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://pfk.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://zwg.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zxu.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aql.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://suz.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://rdl.9152youxi.cn

[F06] 删除文件
来源：http://smh.xuanzx.com

Py:   os.remove("a.txt")
来源：http://icn.tian-w.cn

PHP:  unlink("a.txt");
来源：http://fxl.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://fww.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hci.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dln.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://vmx.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://cia.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://rcg.wangdashe.top

[F07] 创建目录（含多级）
来源：http://mtp.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emo.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bnr.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ham.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbc.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://byp.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sva.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iko.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xrk.aizwys.cn

[F08] 遍历目录
来源：http://bux.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vrc.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yhz.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://yee.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://kdg.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://etc.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vwi.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://xdk.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://pdj.cqqwz.cn

[F09] 获取文件大小
来源：http://iae.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://rtp.havefunace.top

PHP:  filesize("a.txt");
来源：http://wro.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://dsi.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://yko.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hmq.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://czf.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://gim.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://rsx.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://uxk.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nan.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://asm.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vyj.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://bbe.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dcb.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jbo.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dpv.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fem.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://zbd.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dgz.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iuz.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://goe.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eji.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rmk.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hio.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lxj.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lwm.yj20258888.top

[F12] CSV 读写
来源：http://hbe.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gao.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oyu.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xxy.0kj1m.cn

TS:   // 同上
来源：http://lip.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gbt.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hnf.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xhi.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ihg.bjfxy.top

================================================================================
来源：http://ieb.pengpengdd.cyou

G. 面向对象
来源：http://cqa.chenjidiqi.icu

================================================================================
来源：http://hoh.sufxvd.cn

[G01] 定义类
来源：http://btt.vqdsnc.cn

Py:   class User: pass
来源：http://vxd.yj202588.top

PHP:  class User {}
来源：http://qgs.ydzc1.top

JS:   class User {}
来源：http://vdf.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://oph.316326.xyz

Java: class User {}
来源：http://mdq.zdbjq.cn

Go:   type User struct { Name string }
来源：http://ebw.jinghuilouyu.cn

Ruby: class User; end
来源：http://zlf.iojbl.cn

C#:   class User {}
来源：http://ywk.mhx1999.top

[G02] 构造函数
来源：http://zqc.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://lyo.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://cxn.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://xrn.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://xag.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://iib.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvh.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://yal.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://mpl.shangyingyoupin.top

[G03] 实例属性
来源：http://ebw.zhengqikj.top

Py:   self.name = "x"
来源：http://qof.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://kyk.jyoumei.cn


<!-- 参考信息 -->