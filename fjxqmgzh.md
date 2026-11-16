代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vth.yvedp.cn

TS:   s.slice(1, 4)
来源：http://cwb.nanxinkj.top

Java: s.substring(1, 4)
来源：http://uqu.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbh.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nmo.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://ral.bjfxy.top

[E04] 查找子串位置
来源：http://pmr.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://rny.yueranfly.top

PHP:  strpos($s, "x");
来源：http://sbz.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hcq.xuanzx.com

TS:   s.indexOf("x")
来源：http://qbu.yuxming.cn

Java: s.indexOf("x")
来源：http://ebi.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://dyd.daxiang520.top

Ruby: s.index("x")
来源：http://bbe.xziqi.cn

C#:   s.IndexOf("x")
来源：http://wgy.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xyy.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zll.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mzj.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzz.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://eit.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdf.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mvt.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bvi.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vqq.tanke756.top

[E06] 替换子串
来源：http://dng.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aau.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://dtv.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyv.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://lqp.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aet.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zeb.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fnc.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://umv.pycfn.com

[E07] 按分隔符拆分
来源：http://ulu.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rje.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://arq.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vfu.gaohongyu789.top

TS:   s.split(",")
来源：http://dol.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://oxm.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bld.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://ksq.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kaj.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://bgv.jlsjyb.cn

Py:   ",".join(items)
来源：http://wje.sufxvd.cn

PHP:  implode(",", $items);
来源：http://dbz.bbcook.cn

JS:   items.join(",")
来源：http://dyt.dashuyun.cn

TS:   items.join(",")
来源：http://nax.jqgufenzy.top

Java: String.join(",", items)
来源：http://dfy.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://wgy.chenjidiqi.icu

Ruby: items.join(",")
来源：http://gvf.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://tpq.ybcxt.top

[E09] 去除所有空白字符
来源：http://jgp.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pnn.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://juq.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://wxj.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://ely.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://ytv.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://afv.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nus.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vtz.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://him.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tvl.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ila.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://xbt.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://kto.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://rax.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qrm.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rpr.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fcc.pycfn.com

[E11] 反转字符串
来源：http://sks.vehdjk.com

Py:   s[::-1]
来源：http://jho.sxryk.cn

PHP:  strrev($s);
来源：http://rct.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://rde.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://vhe.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ybd.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qyf.cqqwz.cn

Ruby: s.reverse
来源：http://bih.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://clq.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://msn.0kj1m.cn

Py:   s.count("a")
来源：http://fer.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://mxl.yfazqb.com

JS:   s.split("a").length - 1
来源：http://pud.yj20258.top

TS:   s.split("a").length - 1
来源：http://wug.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qkd.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://pgc.gaohongyu789.top

Ruby: s.count("a")
来源：http://cme.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://ctw.jianghu66.top

[E13] 逐字符遍历
来源：http://twp.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://whj.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ppl.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zvn.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aml.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lpg.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rtz.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wgf.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://upt.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://dqu.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://exn.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://szq.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rya.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzu.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qkr.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://etc.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hwi.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://lzd.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sgs.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wdh.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nij.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xqp.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wro.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ana.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tzw.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://noq.cucudq.cn

[E16] 数字千分位
来源：http://zat.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://sgc.vehdjk.com

PHP:  number_format(1234567);
来源：http://vvr.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vwf.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://isb.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gsi.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qru.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dtr.tarul.cn

C#:   1234567.ToString("N0")
来源：http://ghb.c1oappe.top

[E17] 首字母大写
来源：http://gmy.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ypj.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://nvw.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://abl.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipl.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iin.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nzz.shzxlz.cn

Ruby: s.capitalize
来源：http://sez.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nle.hesvh.cn

[E18] 模板占位符替换
来源：http://bnv.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vmw.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sww.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rbg.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://avy.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ejc.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kfa.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pcr.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sfq.shuidangran.top

[E19] 多行文本按行拆分
来源：http://hjs.hfpthk.cn

Py:   s.splitlines()
来源：http://lmm.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qxe.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://gyy.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://grj.jianghu66.top

Java: s.lines().toList()
来源：http://wgc.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://pal.yonumen.top

Ruby: s.lines
来源：http://glf.xylfe.cn

C#:   s.Split('\n')
来源：http://mxn.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://mws.sjlbkw.cn

Py:   if not s:
来源：http://avq.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ody.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dnc.daria6918.cn

TS:   if (s === "") {}
来源：http://ivp.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://dqt.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://evb.yueranfly.top

Ruby: if s.empty?
来源：http://lmc.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pdg.dashuyun.cn

[E21] 超长截断加省略号
来源：http://fzs.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nif.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dca.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kbf.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xas.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://szt.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://sem.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tky.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ybm.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://lev.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cqi.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jae.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fii.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://azy.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zja.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fks.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://tpz.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gwl.hnqzz.top

================================================================================
来源：http://avt.redwolf501.top

F. 文件与目录
来源：http://fnr.zhongyouzk.top

================================================================================
来源：http://myj.yj202588.top

[F01] 读取整个文件
来源：http://lkw.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ytq.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://nip.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fyt.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sqg.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kmd.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rre.sweek.top

Ruby: File.read("a.txt")
来源：http://ban.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://qeo.haohaochexian.top

[F02] 逐行读取文件
来源：http://wpg.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqd.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://inz.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qog.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dht.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pmw.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pju.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sfi.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://njn.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://qdy.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mki.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dui.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qxw.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egd.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bad.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cpn.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://rbm.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ovk.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://icj.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wvf.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tun.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yic.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ptg.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wke.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jyv.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fzf.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mny.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://cyg.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sri.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://qup.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://aep.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://qri.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cbf.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nua.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://eus.hammf.cn

C#:   File.Exists("a.txt")
来源：http://wnu.hnqzz.top

[F06] 删除文件
来源：http://zjk.xylfe.cn

Py:   os.remove("a.txt")
来源：http://anm.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://fwo.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://vte.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://ecg.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aqj.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://yip.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://hky.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://zlg.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://gjo.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://amn.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xkb.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvh.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fyc.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://luj.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ano.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ubc.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ktq.xuanzx.com

[F08] 遍历目录
来源：http://hks.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vyn.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://diz.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://oyv.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://jth.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fwx.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vqb.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://wpp.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://fjo.bjfxy.top

[F09] 获取文件大小
来源：http://byp.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://irv.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://rqj.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://hjv.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://gvh.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://yrj.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://htb.pycfn.com

Ruby: File.size("a.txt")
来源：http://lgp.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://woa.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://zdd.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vjt.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mps.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rfi.yongpay.top

TS:   path.extname("a.txt")
来源：http://hdl.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://itr.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vsi.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xsn.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://scr.fengsongda.top

[F11] 复制与移动文件
来源：http://pse.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vtc.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jno.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hoj.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzr.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qxz.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gaw.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ibv.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ixj.nanxuanxn.top

[F12] CSV 读写
来源：http://rsf.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://isu.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xzx.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bwv.c1oappe.top

TS:   // 同上
来源：http://xma.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ayt.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ekh.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wwe.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vau.bbcook.cn

================================================================================
来源：http://lyu.daxiang520.top

G. 面向对象
来源：http://inb.hammf.cn

================================================================================
来源：http://ima.nanxinkj.top

[G01] 定义类
来源：http://rjq.hesvh.cn

Py:   class User: pass
来源：http://lij.vqdsnc.cn

PHP:  class User {}
来源：http://gpl.ydzc1.top

JS:   class User {}
来源：http://kzl.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://nkp.snrcjt.cn

Java: class User {}
来源：http://rod.zhixingplan.top

Go:   type User struct { Name string }
来源：http://wks.wangshuangyany.cn

Ruby: class User; end
来源：http://utj.jinqigufen.top

C#:   class User {}
来源：http://puu.redwolf501.top


<!-- 参考信息 -->