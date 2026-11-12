代发 wailian999

Go:   strings.Index(s, "x")
来源：http://klf.zhijiandao.cn

Ruby: s.index("x")
来源：http://atu.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://qzx.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://wyw.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ykv.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eeg.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldf.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gkl.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jom.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://job.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gac.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yia.nanxuanxn.top

[E06] 替换子串
来源：http://ykh.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tfm.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://qgc.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pdl.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://vli.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kfv.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://awb.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cqp.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://bap.zhixingplan.top

[E07] 按分隔符拆分
来源：http://utf.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://myd.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gws.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qwa.ybcxt.top

TS:   s.split(",")
来源：http://bgo.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xne.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ntw.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://ygq.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qzw.ydzc1.top

[E08] 数组按分隔符合并
来源：http://vni.zhoulong.xyz

Py:   ",".join(items)
来源：http://aaa.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://aou.yj20258888.top

JS:   items.join(",")
来源：http://gdj.redwolf501.top

TS:   items.join(",")
来源：http://jbk.pengpengdd.cyou

Java: String.join(",", items)
来源：http://pkx.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://zaz.hnqzz.top

Ruby: items.join(",")
来源：http://xhl.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://las.snrcjt.cn

[E09] 去除所有空白字符
来源：http://dwo.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fhj.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ppp.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://mof.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://wbq.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://lng.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ifp.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://moe.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rtk.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://nua.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vqd.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tiz.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://tbm.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://jwk.pycfn.com

Java: String.format("%03d", 7)
来源：http://mem.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fey.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kpa.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pta.jinqigfzy.top

[E11] 反转字符串
来源：http://fpp.hammf.cn

Py:   s[::-1]
来源：http://ivw.9152youxi.cn

PHP:  strrev($s);
来源：http://pob.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://wtk.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://rpi.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jik.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rri.cashguo.top

Ruby: s.reverse
来源：http://ysg.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fua.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://ihf.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://pri.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://oop.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://dyw.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://ocm.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dor.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://crn.nanxinkj.top

Ruby: s.count("a")
来源：http://lnd.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://unf.fengsongda.top

[E13] 逐字符遍历
来源：http://gpq.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://xzu.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uqi.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jph.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ifn.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rrv.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mej.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://orf.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://umd.xziqi.cn

[E14] URL 编码与 Base64
来源：http://qel.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pfj.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xux.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rji.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yib.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nrw.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iwu.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://onr.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://umz.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://aam.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kix.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pgr.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ach.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mof.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://skz.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fzv.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vys.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qpc.gaohongyu789.top

[E16] 数字千分位
来源：http://tcj.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://tmo.ydzc1.top

PHP:  number_format(1234567);
来源：http://jju.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zrp.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nqh.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxs.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pqd.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cer.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://thy.nanxuanxn.top

[E17] 首字母大写
来源：http://cwf.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qcq.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tmp.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gaw.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ulr.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zts.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dil.ctjpmb.com

Ruby: s.capitalize
来源：http://sdq.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://soe.zycfv.cn

[E18] 模板占位符替换
来源：http://lwf.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pfa.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bir.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://twt.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://afr.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ior.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://alj.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tof.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hdv.birdmap.top

[E19] 多行文本按行拆分
来源：http://eue.sxryk.cn

Py:   s.splitlines()
来源：http://szo.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyv.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://sgb.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://oja.hnxiangtu.top

Java: s.lines().toList()
来源：http://qtk.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://uoa.havefunace.top

Ruby: s.lines
来源：http://kwv.yj20258.top

C#:   s.Split('\n')
来源：http://zcg.sxryk.cn

[E20] 判断字符串是否为空
来源：http://xxh.hywenlv.cn

Py:   if not s:
来源：http://osz.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghy.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ath.nwbrower.top

TS:   if (s === "") {}
来源：http://efg.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://qth.9152youxi.cn

Go:   if s == "" {}
来源：http://ckh.cdnleiting.top

Ruby: if s.empty?
来源：http://eru.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uuy.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://bok.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bmq.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://myb.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vif.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nmb.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bqs.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://raq.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sam.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qdn.tian-w.cn

[E22] 字节长度与字符长度
来源：http://was.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yvy.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oid.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://evv.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpt.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fab.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dzy.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://uqc.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bna.xuanzx.com

================================================================================
来源：http://oqz.chenzaomai.com

F. 文件与目录
来源：http://hdz.redwolf501.top

================================================================================
来源：http://vsa.andypj.xyz

[F01] 读取整个文件
来源：http://fqi.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lzm.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://xss.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://elo.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dua.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rse.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hti.yuxming.cn

Ruby: File.read("a.txt")
来源：http://rau.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://mun.yanxiufei.cn

[F02] 逐行读取文件
来源：http://hqm.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qwa.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zjq.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjy.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yev.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ouw.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ukw.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fzp.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uef.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://bel.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mzz.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ifa.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egv.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vox.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vec.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tds.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://qgf.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hzn.snrcjt.cn

[F04] 追加写入文件
来源：http://ybk.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://trc.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rvb.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pdg.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jns.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xud.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lsc.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbn.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xjs.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://wgt.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oyh.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://wdx.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://cvz.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://vtj.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ssf.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hkm.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://ncr.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://mkd.316326.xyz

[F06] 删除文件
来源：http://qjm.guannengcc.top

Py:   os.remove("a.txt")
来源：http://phj.tian-w.cn

PHP:  unlink("a.txt");
来源：http://kqu.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ois.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://kkt.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://keg.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://vbs.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://mew.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://igq.tian-w.cn

[F07] 创建目录（含多级）
来源：http://lvp.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jsf.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iag.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eag.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eyi.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gco.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oxm.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgl.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gdc.xinyue.icu

[F08] 遍历目录
来源：http://ryr.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ovo.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sqt.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://thn.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://yzu.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fat.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xok.ivvv.top

Ruby: Dir.children("dir")
来源：http://jga.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://qih.yanxiufei.cn

[F09] 获取文件大小
来源：http://xma.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://kjt.ydzc1.top

PHP:  filesize("a.txt");
来源：http://iwl.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://rmw.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://plh.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://ort.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cct.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://eks.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://bpa.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://wxv.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kel.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vyh.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yeo.uphjek.com

TS:   path.extname("a.txt")
来源：http://jnt.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jds.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wga.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vap.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mov.cdnleiting.top

[F11] 复制与移动文件
来源：http://ovw.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pwv.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dxm.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzc.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmf.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://huy.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xzr.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hms.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gtc.c1oappe.top

[F12] CSV 读写
来源：http://lom.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgt.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fbi.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lov.zhixingplan.top

TS:   // 同上
来源：http://bvn.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cfh.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fhm.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gjn.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dqp.nanxinkj.top

================================================================================
来源：http://pzs.vqdsnc.cn

G. 面向对象
来源：http://wvo.chenlongwang.top

================================================================================
来源：http://tju.gaohongyu789.top

[G01] 定义类
来源：http://bvg.nanxinkj.top

Py:   class User: pass
来源：http://mkf.yuanzhike.top

PHP:  class User {}
来源：http://trz.jiagoushi.top

JS:   class User {}
来源：http://ogz.cashguo.top

TS:   class User { name: string = ""; }
来源：http://tgq.fehbvm.com

Java: class User {}
来源：http://bdq.fehbvm.com

Go:   type User struct { Name string }
来源：http://prm.chenzaomai.com

Ruby: class User; end
来源：http://try.meibo888.top

C#:   class User {}
来源：http://qyc.haohaochexian.top

[G02] 构造函数
来源：http://gau.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://ibh.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://vlm.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://cnt.yj20258.top

TS:   constructor(public name: string) {}
来源：http://oys.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://xyd.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyt.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://czo.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://yny.shzxlz.cn

[G03] 实例属性
来源：http://ris.hongshengwenyu.top

Py:   self.name = "x"
来源：http://vfr.daria6918.cn

PHP:  public string $name = "x";
来源：http://vsy.zhongyouzk.top


<!-- 参考信息 -->