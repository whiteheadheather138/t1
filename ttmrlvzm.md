代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ery.cdnleiting.top

[E03] 截取子串
来源：http://cte.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yee.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tqg.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pxt.tian-w.cn

TS:   s.slice(1, 4)
来源：http://hue.xinyue.icu

Java: s.substring(1, 4)
来源：http://msq.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pwy.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://qxg.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://kht.ehwqpu.com

[E04] 查找子串位置
来源：http://uqk.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://rut.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://mxt.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vrh.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://mti.vqdsnc.cn

Java: s.indexOf("x")
来源：http://xyl.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://jfr.tianlin.xyz

Ruby: s.index("x")
来源：http://dsz.guannengcc.top

C#:   s.IndexOf("x")
来源：http://gam.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yki.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kax.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ovc.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pvt.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://ait.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ykz.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ube.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yyn.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdb.ppjwa.cn

[E06] 替换子串
来源：http://sxs.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qry.guowangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://yvg.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkj.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://zzv.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yta.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://liz.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nts.cashguo.top

C#:   s.Replace("a", "b")
来源：http://xzk.hywenlv.cn

[E07] 按分隔符拆分
来源：http://ukq.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gmj.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rhw.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zqg.gogol.net.cn

TS:   s.split(",")
来源：http://xnn.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://owa.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nbz.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://vhf.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gck.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://fam.dashuyun.cn

Py:   ",".join(items)
来源：http://bit.kuanghao11.cn

PHP:  implode(",", $items);
来源：http://oos.yongpay.top

JS:   items.join(",")
来源：http://rff.cqqwz.cn

TS:   items.join(",")
来源：http://ajm.nanxinkj.top

Java: String.join(",", items)
来源：http://phu.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://fsn.jinqigufen.top

Ruby: items.join(",")
来源：http://rny.yueranfly.top

C#:   string.Join(",", items)
来源：http://asb.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://fqy.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jql.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jtp.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://nod.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://bys.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://cam.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zsh.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vix.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://agd.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://xxy.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://avy.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qwx.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://dbk.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://wne.sweek.top

Java: String.format("%03d", 7)
来源：http://irj.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jfg.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vav.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxl.xuetiantiany.cn

[E11] 反转字符串
来源：http://nec.aizwys.cn

Py:   s[::-1]
来源：http://wgl.meibo888.top

PHP:  strrev($s);
来源：http://jhl.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://bkq.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://uon.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://vni.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://pmz.ehwqpu.com

Ruby: s.reverse
来源：http://ofr.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://jna.meibo888.top

[E12] 统计某字符出现次数
来源：http://jbv.dashuyun.cn

Py:   s.count("a")
来源：http://ytc.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://cdj.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://dgj.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://axt.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dzw.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://uda.xziqi.cn

Ruby: s.count("a")
来源：http://jpz.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://mhp.cdnleiting.top

[E13] 逐字符遍历
来源：http://zwu.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://ieu.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eoo.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hkj.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://zwm.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mit.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mkn.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tcj.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rbl.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://zst.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dsf.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzo.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kzr.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dfg.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ypi.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oox.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eni.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://huo.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://dip.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://yys.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jhs.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://azn.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gav.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eto.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oqc.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uag.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cif.ehwqpu.com

[E16] 数字千分位
来源：http://tgl.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://lfm.c1oappe.top

PHP:  number_format(1234567);
来源：http://emp.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://haa.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://nqm.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myp.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pct.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yub.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://zcr.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://tft.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tlf.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qct.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://unx.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltd.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tsn.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sen.birdmap.top

Ruby: s.capitalize
来源：http://kue.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gmd.birdmap.top

[E18] 模板占位符替换
来源：http://kqa.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wpl.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://owb.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qfy.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nzg.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://deq.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nex.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lrc.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mok.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://afh.hysaishi.cn

Py:   s.splitlines()
来源：http://ita.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qmq.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://qjz.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://ais.smart0.xyz

Java: s.lines().toList()
来源：http://qds.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://tue.sufxvd.cn

Ruby: s.lines
来源：http://acp.snrcjt.cn

C#:   s.Split('\n')
来源：http://pwy.tanke756.top

[E20] 判断字符串是否为空
来源：http://fcj.redwolf501.top

Py:   if not s:
来源：http://uel.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lgt.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ttk.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://jlr.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://rej.sweek.top

Go:   if s == "" {}
来源：http://gam.nanxuanxn.top

Ruby: if s.empty?
来源：http://ufe.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hsx.zdqjudy.top

[E21] 超长截断加省略号
来源：http://awy.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kxq.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qwj.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fcd.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kxr.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uwb.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://zzf.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nau.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hyu.aizwys.cn

[E22] 字节长度与字符长度
来源：http://anq.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://esb.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ybd.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxx.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xhw.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhj.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ign.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://oil.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xnc.zdbjq.cn

================================================================================
来源：http://gsk.daria6918.cn

F. 文件与目录
来源：http://bth.tanke756.top

================================================================================
来源：http://aga.shzxlz.cn

[F01] 读取整个文件
来源：http://qzu.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ohh.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://rqq.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oty.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xpe.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mav.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cej.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://nja.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://mve.sxryk.cn

[F02] 逐行读取文件
来源：http://hcn.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ydd.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ozf.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ylp.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvl.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mjm.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mpv.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oap.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wmj.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://rpg.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdg.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://bqr.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzk.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://buj.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jbw.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qnh.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://bsk.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rna.ctjpmb.com

[F04] 追加写入文件
来源：http://lrv.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zhx.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qye.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyr.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hba.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xfu.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pqz.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://swn.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hdg.sweek.top

[F05] 判断文件或目录是否存在
来源：http://hpr.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://enu.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://pee.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://eqn.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://nul.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jpx.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ejl.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://zav.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://tvr.xinyue.icu

[F06] 删除文件
来源：http://thn.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://wwj.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://kam.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://jym.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://yqm.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xzc.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://mgj.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://vmo.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://adk.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://lhh.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wcg.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sac.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oof.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxh.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tlk.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uwi.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mgw.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jsf.hnxiangtu.top

[F08] 遍历目录
来源：http://ycv.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gmy.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qnz.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://bxc.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://cdc.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cgg.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uzr.sxryk.cn

Ruby: Dir.children("dir")
来源：http://mgg.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://ocy.yanxiufei.cn

[F09] 获取文件大小
来源：http://ead.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://bir.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://yag.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://xhe.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://rbb.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wjr.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdt.c1oappe.top

Ruby: File.size("a.txt")
来源：http://rid.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://nee.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://xkn.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ryg.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dqs.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dgb.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://fzu.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pmk.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xas.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lnh.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jte.cheryme.top

[F11] 复制与移动文件
来源：http://fgw.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://umn.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qyg.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xhv.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://noc.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dyb.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zcz.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sra.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eey.daxiang520.top

[F12] CSV 读写
来源：http://err.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mlq.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbq.snrcjt.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hpu.fanxiaobao.xyz

TS:   // 同上
来源：http://cav.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://smb.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jyb.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ysr.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kdp.fengsongda.top

================================================================================
来源：http://wny.cheryme.top

G. 面向对象
来源：http://wwi.hysaishi.cn

================================================================================
来源：http://jrw.chenzaomai.com

[G01] 定义类
来源：http://fbw.aizwys.cn

Py:   class User: pass
来源：http://yio.uphjek.com

PHP:  class User {}
来源：http://otn.wangshuangyany.cn

JS:   class User {}
来源：http://jlb.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://let.chenzaomai.com


<!-- 参考信息 -->