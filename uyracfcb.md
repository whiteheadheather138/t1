代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://pja.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://ihb.wangdashe.top

[E04] 查找子串位置
来源：http://elq.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://jnj.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://wvf.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kvb.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://iry.zhongyouzk.top

Java: s.indexOf("x")
来源：http://wnk.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://ezt.daxiang520.top

Ruby: s.index("x")
来源：http://fuv.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://ara.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gam.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qih.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://syh.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rjv.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mvk.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yeo.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hwx.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://quz.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bim.wangdashe.top

[E06] 替换子串
来源：http://hkv.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ktu.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://hgq.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhq.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://uvc.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ken.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gds.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umu.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://bvc.havefunace.top

[E07] 按分隔符拆分
来源：http://ndp.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://thh.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mij.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://hnt.0kj1m.cn

TS:   s.split(",")
来源：http://ttv.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xxl.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wgp.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://efb.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kdr.sweek.top

[E08] 数组按分隔符合并
来源：http://frd.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://kjx.hywenlv.cn

PHP:  implode(",", $items);
来源：http://oxs.dianchejie.cn

JS:   items.join(",")
来源：http://zcb.yueranfly.top

TS:   items.join(",")
来源：http://fff.fzhhl.top

Java: String.join(",", items)
来源：http://ewe.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://mhv.ydzc1.top

Ruby: items.join(",")
来源：http://zqj.haohaochexian.top

C#:   string.Join(",", items)
来源：http://iaj.zhixingplan.top

[E09] 去除所有空白字符
来源：http://tua.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://srl.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ipz.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://nag.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://vfs.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://cot.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fzl.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mjr.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fxm.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://fap.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ptd.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qhp.sweek.top

JS:   "7".padStart(3, "0")
来源：http://oov.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://eoa.meibo888.top

Java: String.format("%03d", 7)
来源：http://tlb.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tcb.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://doo.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yet.yj20258888.top

[E11] 反转字符串
来源：http://wme.svipenyu.cn

Py:   s[::-1]
来源：http://zjw.chenlongwang.top

PHP:  strrev($s);
来源：http://slw.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://qcu.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://nsx.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://isz.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iyb.jiagoushi.top

Ruby: s.reverse
来源：http://dyj.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://hxq.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://eis.ybcxt.top

Py:   s.count("a")
来源：http://yik.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://vjc.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://mrn.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://llm.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zrr.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://itd.yvedp.cn

Ruby: s.count("a")
来源：http://sdv.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://reb.ivvv.top

[E13] 逐字符遍历
来源：http://ydy.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://yoh.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qso.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rkh.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gsb.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mjj.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cly.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://wdn.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hwg.mhx1999.top

[E14] URL 编码与 Base64
来源：http://dbp.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ojw.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mjn.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ots.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zya.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mrz.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vsk.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qes.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://omj.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://afa.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ltf.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhr.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://adc.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dvu.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ltg.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lpy.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mdb.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lad.yangfankeji.com

[E16] 数字千分位
来源：http://wya.52xcode.cn

Py:   f"{1234567:,}"
来源：http://guu.haohaochexian.top

PHP:  number_format(1234567);
来源：http://vvc.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cks.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nwx.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://klc.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gve.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kpn.pycfn.com

C#:   1234567.ToString("N0")
来源：http://avq.zhongyouzk.top

[E17] 首字母大写
来源：http://xrg.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://isc.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rfq.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://csj.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wew.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ptt.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jtl.cqqwz.cn

Ruby: s.capitalize
来源：http://jij.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pyr.jiagoushi.top

[E18] 模板占位符替换
来源：http://bcj.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bfd.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fux.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tdv.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://veu.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zfs.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vrr.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wpu.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wud.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://hge.birdmap.top

Py:   s.splitlines()
来源：http://ubc.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ilv.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://dss.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://rlu.nanxinkj.top

Java: s.lines().toList()
来源：http://bcf.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://bsn.zhaomingkeji.xyz

Ruby: s.lines
来源：http://nuq.tian-w.cn

C#:   s.Split('\n')
来源：http://zmk.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://rah.jinqigufen.top

Py:   if not s:
来源：http://kkt.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qdl.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wqh.iojbl.cn

TS:   if (s === "") {}
来源：http://xmd.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://pum.yj202588.top

Go:   if s == "" {}
来源：http://xep.jqgufenzy.top

Ruby: if s.empty?
来源：http://vhg.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hpd.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://tai.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lpw.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://muj.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wik.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qre.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dgv.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://xrf.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yfe.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://clq.bbcook.cn

[E22] 字节长度与字符长度
来源：http://oqx.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pfn.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://twq.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yiy.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrk.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gdj.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ppr.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://akv.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://obz.yueranfly.top

================================================================================
来源：http://rhh.epnwcf.com

F. 文件与目录
来源：http://uei.cdnleiting.top

================================================================================
来源：http://ufv.chenjidiqi.icu

[F01] 读取整个文件
来源：http://ufe.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sik.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://fmn.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vfo.zhaomingkeji.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://peu.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjl.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xrp.fehbvm.com

Ruby: File.read("a.txt")
来源：http://zur.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://yac.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://zea.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bmi.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xit.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gzd.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svy.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sgf.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://czs.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oum.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iwx.meibo888.top

[F03] 写入文件（覆盖）
来源：http://drn.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qlx.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cix.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxr.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://viz.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cep.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zoz.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://xwq.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rhd.tarul.cn

[F04] 追加写入文件
来源：http://sne.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pli.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jlv.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrm.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ooh.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jsg.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dln.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qcn.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gym.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://ewq.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vde.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://kwq.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://nbd.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://cut.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aaw.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iuc.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://uda.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://wwq.chenlongwang.top

[F06] 删除文件
来源：http://caw.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://vzq.fktsv.cn

PHP:  unlink("a.txt");
来源：http://yod.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://kgi.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://xzi.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://edq.tarul.cn

Go:   os.Remove("a.txt")
来源：http://ojr.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://ahk.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://fpt.guannengcc.top

[F07] 创建目录（含多级）
来源：http://hto.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jyk.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vuc.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbw.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqm.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xkv.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aov.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ymb.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ime.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://zjr.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxc.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hor.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://gbb.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://wfc.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vgx.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gah.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://lif.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://usx.hammf.cn

[F09] 获取文件大小
来源：http://szu.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://cei.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://npx.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://kmw.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://fhp.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://uzh.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hwk.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://nkz.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://iiy.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://wqy.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gsz.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lux.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mae.vehdjk.com

TS:   path.extname("a.txt")
来源：http://ajs.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aee.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whf.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vke.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://isv.yfazqb.com

[F11] 复制与移动文件
来源：http://leh.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rne.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kqh.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zds.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzt.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aqj.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://van.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xaw.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tmn.shuidangran.top

[F12] CSV 读写
来源：http://dem.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rhi.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zcw.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrs.shuidangran.top

TS:   // 同上
来源：http://zkv.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pye.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cvr.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zax.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vtz.cucudq.cn

================================================================================
来源：http://pri.yvedp.cn

G. 面向对象
来源：http://kdg.cheryme.top

================================================================================
来源：http://xmz.wangshuangyany.cn

[G01] 定义类
来源：http://sij.yonumen.top

Py:   class User: pass
来源：http://hhu.ehwqpu.com

PHP:  class User {}
来源：http://ino.fanxiaobao.xyz

JS:   class User {}
来源：http://fto.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://zfg.wangdashe.top

Java: class User {}
来源：http://caj.yj202588.top

Go:   type User struct { Name string }
来源：http://sid.yuxming.cn

Ruby: class User; end
来源：http://klk.wangdashe.top

C#:   class User {}
来源：http://lze.zhengqikj.top

[G02] 构造函数
来源：http://ljm.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://pja.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://gwy.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://bix.hywenlv.cn


<!-- 参考信息 -->