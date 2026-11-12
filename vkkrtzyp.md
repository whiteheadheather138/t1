代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gez.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zjd.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ieg.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bxz.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xre.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mal.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yji.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mni.epnwcf.com

[E06] 替换子串
来源：http://kaz.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kad.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://bqn.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eri.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://lgp.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnw.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aox.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wqw.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://bfp.52xcode.cn

[E07] 按分隔符拆分
来源：http://pow.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cia.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ozk.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://akl.yuxming.cn

TS:   s.split(",")
来源：http://hlm.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://yqn.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://who.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://vul.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uoo.cucudq.cn

[E08] 数组按分隔符合并
来源：http://ted.guowangkeji.top

Py:   ",".join(items)
来源：http://ppu.aibaodan.cn

PHP:  implode(",", $items);
来源：http://eri.gaohongyu789.top

JS:   items.join(",")
来源：http://ykq.havefunace.top

TS:   items.join(",")
来源：http://ius.sjlbkw.cn

Java: String.join(",", items)
来源：http://cfk.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://llk.andypj.xyz

Ruby: items.join(",")
来源：http://pzy.nanxinkj.top

C#:   string.Join(",", items)
来源：http://hxx.yvedp.cn

[E09] 去除所有空白字符
来源：http://zuv.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vyq.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iib.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://noj.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://mqp.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://ada.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cuw.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://ene.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tlt.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://tpk.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oio.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nnc.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://jsx.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://dcp.yueranfly.top

Java: String.format("%03d", 7)
来源：http://rpr.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fta.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cru.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ffi.kuanghao11.cn

[E11] 反转字符串
来源：http://vgd.zdqjudy.top

Py:   s[::-1]
来源：http://sql.meibo888.top

PHP:  strrev($s);
来源：http://akg.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://ula.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://vft.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sho.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hjs.tarul.cn

Ruby: s.reverse
来源：http://sck.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://jic.pycfn.com

[E12] 统计某字符出现次数
来源：http://gjh.guowangkeji.top

Py:   s.count("a")
来源：http://bgu.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://uki.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://nul.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://imi.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xyc.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://ede.hfpthk.cn

Ruby: s.count("a")
来源：http://zbq.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://iey.tianlin.xyz

[E13] 逐字符遍历
来源：http://gob.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://tgz.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xiu.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xkv.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jfb.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bqu.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lrv.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jbv.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qlr.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://aev.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uce.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvj.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhf.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dyx.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sbe.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qtp.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://itx.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gzr.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://gqw.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wnv.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wvo.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lbx.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kpb.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://seq.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bxi.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rtd.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ctw.pycfn.com

[E16] 数字千分位
来源：http://ajs.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://wcf.daxiang520.top

PHP:  number_format(1234567);
来源：http://yec.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kpm.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pfd.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wvu.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ozb.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nsq.tanke756.top

C#:   1234567.ToString("N0")
来源：http://von.yj20258.top

[E17] 首字母大写
来源：http://lqa.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://amq.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cct.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfp.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmj.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pxv.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fsw.gogol.net.cn

Ruby: s.capitalize
来源：http://owr.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://clf.yj20258888.top

[E18] 模板占位符替换
来源：http://cbj.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggf.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yxg.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://awi.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dgb.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://les.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onh.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zbq.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sqp.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://azn.hammf.cn

Py:   s.splitlines()
来源：http://aaq.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cmc.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://hdi.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://axe.dianchejie.cn

Java: s.lines().toList()
来源：http://eie.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://tqb.bbcook.cn

Ruby: s.lines
来源：http://zei.birdmap.top

C#:   s.Split('\n')
来源：http://nyr.yfazqb.com

[E20] 判断字符串是否为空
来源：http://epb.redwolf501.top

Py:   if not s:
来源：http://jin.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zgh.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cdn.sufxvd.cn

TS:   if (s === "") {}
来源：http://pqm.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://pad.hesvh.cn

Go:   if s == "" {}
来源：http://euk.xylfe.cn

Ruby: if s.empty?
来源：http://cto.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xad.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://que.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fjo.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qno.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bso.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mca.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yfm.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://xbh.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bux.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rml.xinyue.icu

[E22] 字节长度与字符长度
来源：http://lct.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gxm.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqx.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://olu.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ici.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wdl.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fud.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://yif.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bpj.vehdjk.com

================================================================================
来源：http://kms.9152youxi.cn

F. 文件与目录
来源：http://qdv.feifeiyinyue.top

================================================================================
来源：http://vig.snrcjt.cn

[F01] 读取整个文件
来源：http://fia.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qoq.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://zgw.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rpd.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vdb.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://blg.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wok.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://hur.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://evb.ctjpmb.com

[F02] 逐行读取文件
来源：http://bco.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqq.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rks.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvm.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ivb.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rbf.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tmu.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fvn.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uul.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://ikp.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pkf.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wqj.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpf.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qbu.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kwi.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lff.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://jnk.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qig.cashguo.top

[F04] 追加写入文件
来源：http://lrn.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vsa.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ejm.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xou.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bxg.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://skw.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtn.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mcx.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qzk.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://pij.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gox.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://omx.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://der.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://upc.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xyq.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fss.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://rqg.sweek.top

C#:   File.Exists("a.txt")
来源：http://btn.shzxlz.cn

[F06] 删除文件
来源：http://peg.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://pgh.birdmap.top

PHP:  unlink("a.txt");
来源：http://uoc.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://afb.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://kjn.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gpe.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://sha.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://hat.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://gqf.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://dja.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sqn.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tgn.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ikb.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dzq.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ghs.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ktk.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://goq.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wqx.chenzaomai.com

[F08] 遍历目录
来源：http://kyn.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://hxv.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jfv.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://qen.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://xjn.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sgy.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://egc.ivvv.top

Ruby: Dir.children("dir")
来源：http://uts.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://swy.zycfv.cn

[F09] 获取文件大小
来源：http://sbl.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://pxl.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://ukk.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://lms.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://uvn.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zfv.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jid.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://sgg.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://dzu.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://zjz.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fsv.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bux.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://slf.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://hzm.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fvq.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hzl.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://amz.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cgy.jinqigufen.top

[F11] 复制与移动文件
来源：http://vyd.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kjk.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eds.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awi.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fax.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zpc.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://asp.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://afy.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpe.sjlbkw.cn

[F12] CSV 读写
来源：http://pgo.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xfi.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qwu.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ccb.zhaomingkeji.xyz

TS:   // 同上
来源：http://ulj.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkz.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sxx.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xer.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ytn.zdqjudy.top

================================================================================
来源：http://rhp.zhiwuduotai.top

G. 面向对象
来源：http://viy.zdbjq.cn

================================================================================
来源：http://kak.aibaodan.cn

[G01] 定义类
来源：http://mig.ydzc1.top

Py:   class User: pass
来源：http://xuz.shzxlz.cn

PHP:  class User {}
来源：http://qqm.smart0.xyz

JS:   class User {}
来源：http://vtx.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://rzr.svipenyu.cn

Java: class User {}
来源：http://wbb.cheryme.top

Go:   type User struct { Name string }
来源：http://hbt.yuxming.cn

Ruby: class User; end
来源：http://ccs.cucudq.cn

C#:   class User {}
来源：http://igp.sysykeji.top

[G02] 构造函数
来源：http://hfp.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://lbm.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://wgb.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://dly.meibo888.top

TS:   constructor(public name: string) {}
来源：http://gmp.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://bcn.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rim.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://dvz.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://jlr.hfpthk.cn

[G03] 实例属性
来源：http://lks.ydjk.org.cn

Py:   self.name = "x"
来源：http://kbg.hcnkem.com

PHP:  public string $name = "x";
来源：http://ovt.jqgfzy.top

JS:   this.name = "x";
来源：http://oui.chenzaomai.com

TS:   name: string = "x";
来源：http://wjs.xylfe.cn

Java: private String name;
来源：http://bhp.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rbs.yj20258888.top


<!-- 参考信息 -->