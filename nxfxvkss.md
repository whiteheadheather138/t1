代发 wailian999

[E06] 替换子串
来源：http://paf.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://saf.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://kln.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hza.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://nyi.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdd.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fww.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kcj.cashguo.top

C#:   s.Replace("a", "b")
来源：http://jay.hywenlv.cn

[E07] 按分隔符拆分
来源：http://imo.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ext.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ggz.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bth.chenjidiqi.icu

TS:   s.split(",")
来源：http://yuc.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://rnk.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uxq.yongpay.top

Ruby: s.split(",");  s.split
来源：http://dls.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fxw.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://vtw.yuanzhike.top

Py:   ",".join(items)
来源：http://bvj.gotoacloud.top

PHP:  implode(",", $items);
来源：http://cew.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://ouk.bjfxy.top

TS:   items.join(",")
来源：http://dwf.dianchejie.cn

Java: String.join(",", items)
来源：http://tdg.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://yoc.aizwys.cn

Ruby: items.join(",")
来源：http://tbz.hywenlv.cn

C#:   string.Join(",", items)
来源：http://piy.havefunace.top

[E09] 去除所有空白字符
来源：http://rtq.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vik.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yhr.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://euz.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://dwc.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://xrv.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://for.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://lub.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ioi.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://hoq.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xum.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://drj.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://nrf.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://kps.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://zxn.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qes.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qbk.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mpr.aibaodan.cn

[E11] 反转字符串
来源：http://yzp.mhx1999.top

Py:   s[::-1]
来源：http://nmr.yueranfly.top

PHP:  strrev($s);
来源：http://lcj.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://lur.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://kdu.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://buw.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rrm.zhengqikj.top

Ruby: s.reverse
来源：http://abz.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qds.xylfe.cn

[E12] 统计某字符出现次数
来源：http://xxa.gotoacloud.top

Py:   s.count("a")
来源：http://zmn.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://ysx.jianghu66.top

JS:   s.split("a").length - 1
来源：http://whk.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://cbw.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rjr.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://mcw.feifeiyinyue.top

Ruby: s.count("a")
来源：http://did.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://mta.fzhhl.top

[E13] 逐字符遍历
来源：http://aei.yonumen.top

Py:   for ch in s: print(ch)
来源：http://juo.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xud.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vjo.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hcg.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ytv.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xsh.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://naw.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://huo.uphjek.com

[E14] URL 编码与 Base64
来源：http://xyd.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gil.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pub.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xya.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hbl.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zxe.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qwk.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rgj.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxm.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://cpt.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://inh.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hlo.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sym.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lkh.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dpo.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://myg.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmw.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://olo.daxiang520.top

[E16] 数字千分位
来源：http://mjk.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://sgo.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://ymu.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://tiv.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gzw.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gvy.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bth.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ekw.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://jcs.yj20258.top

[E17] 首字母大写
来源：http://ptq.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://coo.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://qcj.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcc.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://doc.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cei.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ren.hcnkem.com

Ruby: s.capitalize
来源：http://pxz.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tuk.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://yye.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://snm.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ipj.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://muw.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gek.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuy.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wbx.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sai.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cci.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://cxf.zhixingplan.top

Py:   s.splitlines()
来源：http://sze.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://usb.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://hde.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://niv.tanke756.top

Java: s.lines().toList()
来源：http://csn.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://msc.guowangkeji.top

Ruby: s.lines
来源：http://hki.chenlongwang.top

C#:   s.Split('\n')
来源：http://rfw.fehbvm.com

[E20] 判断字符串是否为空
来源：http://cqb.vqdsnc.cn

Py:   if not s:
来源：http://uee.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://coq.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://caa.ctjpmb.com

TS:   if (s === "") {}
来源：http://fay.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://osl.fktsv.cn

Go:   if s == "" {}
来源：http://iao.birdmap.top

Ruby: if s.empty?
来源：http://idx.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://afm.havefunace.top

[E21] 超长截断加省略号
来源：http://sgx.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tfe.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jjn.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ypl.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mpu.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://myp.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://mhk.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ahw.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bvp.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://lfw.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrd.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlp.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcu.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://moe.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kab.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pxo.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://vat.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nou.daxiang520.top

================================================================================
来源：http://cbg.shanyushiyangtech.top

F. 文件与目录
来源：http://szg.guowangkeji.top

================================================================================
来源：http://eof.316326.xyz

[F01] 读取整个文件
来源：http://qqs.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sbw.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://rfr.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxb.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://loz.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ybd.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cdk.daria6918.cn

Ruby: File.read("a.txt")
来源：http://dqo.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://xuv.9152youxi.cn

[F02] 逐行读取文件
来源：http://kvb.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dme.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bma.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kyd.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zyg.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fdd.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lld.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fgz.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwn.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://jls.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xdk.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://toj.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mak.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uge.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pzt.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://poo.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://vnz.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://izo.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://kme.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gfe.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ubw.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpe.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dlo.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kyp.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://scd.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fzn.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bhx.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://xio.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mbd.pycfn.com

PHP:  file_exists("a.txt");
来源：http://ibm.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://psk.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://tcu.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://eyy.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gzg.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://ztx.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://tfh.fengsongda.top

[F06] 删除文件
来源：http://spq.fktsv.cn

Py:   os.remove("a.txt")
来源：http://kew.fzhhl.top

PHP:  unlink("a.txt");
来源：http://xep.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tof.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jjo.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kvy.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://bpd.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://rhp.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://fox.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://qoy.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gjo.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://czy.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://opu.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddf.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yoi.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://osg.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cax.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zow.andypj.xyz

[F08] 遍历目录
来源：http://ldc.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zhm.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eni.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://wqi.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://tjp.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gve.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ias.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://dst.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://wbl.yanxiufei.cn

[F09] 获取文件大小
来源：http://dll.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://dju.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://ywp.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://qcp.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://jef.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://cte.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tuo.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://kjz.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://ayn.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://ugg.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gnn.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uve.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yul.iojbl.cn

TS:   path.extname("a.txt")
来源：http://ufq.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yyj.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qeh.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rpl.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vpv.yonumen.top

[F11] 复制与移动文件
来源：http://cjb.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ler.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sqo.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oth.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouy.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cnj.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iko.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xot.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wrc.yongpay.top

[F12] CSV 读写
来源：http://frs.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://frq.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jld.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://brp.jinqigufen.top

TS:   // 同上
来源：http://acz.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oru.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wnw.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vvm.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://bmi.svipenyu.cn

================================================================================
来源：http://mbn.nwbrower.top

G. 面向对象
来源：http://zpy.cashguo.top

================================================================================
来源：http://khl.hammf.cn

[G01] 定义类
来源：http://kkf.jlsjyb.cn

Py:   class User: pass
来源：http://skz.zhijiandao.cn

PHP:  class User {}
来源：http://ecb.zdqjudy.top

JS:   class User {}
来源：http://qot.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://uza.ivvv.top

Java: class User {}
来源：http://xks.redwolf501.top

Go:   type User struct { Name string }
来源：http://zld.jinqigfzy.top

Ruby: class User; end
来源：http://znk.shanyushiyangkeji.top

C#:   class User {}
来源：http://rnm.cdnleiting.top

[G02] 构造函数
来源：http://dxp.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://mua.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://mrk.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://pfk.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://thk.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://ztx.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jjc.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://ytz.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://xbp.ydjk.org.cn

[G03] 实例属性
来源：http://sqj.daxiang520.top

Py:   self.name = "x"
来源：http://zye.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://rrn.chenzaomai.com

JS:   this.name = "x";
来源：http://skd.ivvv.top

TS:   name: string = "x";
来源：http://udy.ydzc1.top

Java: private String name;
来源：http://nun.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wam.vqdsnc.cn

Ruby: @name = "x"
来源：http://ojb.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://eht.zhoulong.xyz

[G04] 定义方法
来源：http://vrc.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://wss.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ooj.yonumen.top

JS:   greet() { return this.name; }
来源：http://stp.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://mjz.zycfv.cn

Java: String greet() { return name; }
来源：http://wry.jianghu66.top


<!-- 参考信息 -->