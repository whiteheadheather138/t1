代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://atn.jyoumei.cn

TS:   s.split(",")
来源：http://inc.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://qns.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vea.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://cpu.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bgu.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://yus.daria6918.cn

Py:   ",".join(items)
来源：http://uvs.haohaochexian.top

PHP:  implode(",", $items);
来源：http://ewe.fktsv.cn

JS:   items.join(",")
来源：http://wad.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://nnp.tanke756.top

Java: String.join(",", items)
来源：http://ivc.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://ybh.jinqigfzy.top

Ruby: items.join(",")
来源：http://rby.dashuyun.cn

C#:   string.Join(",", items)
来源：http://fdb.sweek.top

[E09] 去除所有空白字符
来源：http://aip.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kqc.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aad.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://crs.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://hnl.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://dvj.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qro.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://bdc.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mgb.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://bjf.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ikl.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oma.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://hth.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://usn.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://mtw.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://exm.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dec.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uqn.vqdsnc.cn

[E11] 反转字符串
来源：http://acz.sufxvd.cn

Py:   s[::-1]
来源：http://gct.quarkkingdee.top

PHP:  strrev($s);
来源：http://cyg.pycfn.com

JS:   [...s].reverse().join("")
来源：http://ztg.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://zal.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uuq.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rgs.fzhhl.top

Ruby: s.reverse
来源：http://mbz.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://ord.tanke756.top

[E12] 统计某字符出现次数
来源：http://laf.sxryk.cn

Py:   s.count("a")
来源：http://uiq.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://bcj.havefunace.top

JS:   s.split("a").length - 1
来源：http://kio.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://wyn.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://inm.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://kdg.zycfv.cn

Ruby: s.count("a")
来源：http://vwr.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://mxp.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://kow.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://wui.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yyl.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwx.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qil.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://spi.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nen.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://wdk.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vem.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://buj.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://biv.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aem.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kem.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qjh.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pxa.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxp.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lvm.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ojt.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://nzn.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wsz.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ktm.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mma.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aip.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fdd.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fkt.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tbf.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iyg.tianlin.xyz

[E16] 数字千分位
来源：http://mfe.yj202588.top

Py:   f"{1234567:,}"
来源：http://nzc.yueranfly.top

PHP:  number_format(1234567);
来源：http://qcb.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rzu.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://brd.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://npy.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrn.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://plh.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://bpl.jianghu66.top

[E17] 首字母大写
来源：http://gqy.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fnz.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://jmp.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzk.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bla.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cgi.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xub.0kj1m.cn

Ruby: s.capitalize
来源：http://cyz.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jap.hfpthk.cn

[E18] 模板占位符替换
来源：http://ecc.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqp.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vkt.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nkn.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cfa.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nyg.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pqg.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://omj.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yqr.aizwys.cn

[E19] 多行文本按行拆分
来源：http://pey.guowangkeji.top

Py:   s.splitlines()
来源：http://knc.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cwz.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://adg.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://vdb.sufxvd.cn

Java: s.lines().toList()
来源：http://mlb.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://irt.cheryme.top

Ruby: s.lines
来源：http://eqn.hywenlv.cn

C#:   s.Split('\n')
来源：http://shl.bjfxy.top

[E20] 判断字符串是否为空
来源：http://tya.nwbrower.top

Py:   if not s:
来源：http://hhv.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pur.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ilj.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://mou.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://hzn.shzxlz.cn

Go:   if s == "" {}
来源：http://vut.havefunace.top

Ruby: if s.empty?
来源：http://uwg.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xqy.yj202588.top

[E21] 超长截断加省略号
来源：http://izk.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sgk.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://web.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ibi.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqo.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mzc.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://jdn.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fjq.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ugd.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://kdi.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lzu.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ivt.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqx.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mop.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://frg.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dgs.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://znr.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cef.gogol.net.cn

================================================================================
来源：http://ovn.pycfn.com

F. 文件与目录
来源：http://xax.yonumen.top

================================================================================
来源：http://hlh.snrcjt.cn

[F01] 读取整个文件
来源：http://uoj.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oun.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://lcu.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bdx.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kbf.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gpv.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ece.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://oml.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://wwk.dianchejie.cn

[F02] 逐行读取文件
来源：http://lek.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gmw.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fpf.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyn.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cmv.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://miv.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pzg.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tha.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qnt.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://hxv.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zwy.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gep.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahj.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yeo.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ral.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://chm.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://dkg.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bpq.jianghu66.top

[F04] 追加写入文件
来源：http://otu.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itd.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://loh.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfu.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iyx.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qcn.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ywk.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rzo.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vyy.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://fjv.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hsj.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://fzd.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://rjz.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://wil.jiagoushi.top

Java: Files.exists(Path.of("a.txt"))
来源：http://llv.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xid.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://svy.316326.xyz

C#:   File.Exists("a.txt")
来源：http://hsr.meibo888.top

[F06] 删除文件
来源：http://pnx.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://iyj.daria6918.cn

PHP:  unlink("a.txt");
来源：http://yoi.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jzw.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://unq.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vsc.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://tks.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://fdy.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://okm.ydzc1.top

[F07] 创建目录（含多级）
来源：http://wzk.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kko.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dyb.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ibr.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ade.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uyv.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zgx.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wma.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rqc.yongpay.top

[F08] 遍历目录
来源：http://imu.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vci.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ciz.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://cxr.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://rit.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gen.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ghc.yueranfly.top

Ruby: Dir.children("dir")
来源：http://wfg.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://ied.bbcook.cn

[F09] 获取文件大小
来源：http://rlf.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://hzd.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://wlv.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://txs.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://ooe.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nwo.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://icp.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://syl.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://dny.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://khu.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vjg.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hfw.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yoh.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://bfo.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ryo.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gch.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yol.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ysq.ppjwa.cn

[F11] 复制与移动文件
来源：http://zuc.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rlj.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bjh.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmq.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmg.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://msw.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://goi.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hii.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wch.guannengcc.top

[F12] CSV 读写
来源：http://gvn.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eeg.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nvw.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrx.yueranfly.top

TS:   // 同上
来源：http://loo.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eph.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cyp.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ebz.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://spc.epnwcf.com

================================================================================
来源：http://wto.cucudq.cn

G. 面向对象
来源：http://lma.shuidangran.top

================================================================================
来源：http://prm.cucudq.cn

[G01] 定义类
来源：http://vom.bjfxy.top

Py:   class User: pass
来源：http://rur.0kj1m.cn

PHP:  class User {}
来源：http://keh.yonumen.top

JS:   class User {}
来源：http://fyr.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://svc.tarul.cn

Java: class User {}
来源：http://qil.hesvh.cn

Go:   type User struct { Name string }
来源：http://hqn.fengsongda.top

Ruby: class User; end
来源：http://zdb.ydjk.org.cn

C#:   class User {}
来源：http://hvw.hnxiangtu.top

[G02] 构造函数
来源：http://uhc.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://grd.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://mkm.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://run.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://ebp.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://der.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wgk.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://rnq.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://czw.dashuyun.cn

[G03] 实例属性
来源：http://wbb.yuxming.cn

Py:   self.name = "x"
来源：http://krj.aizwys.cn

PHP:  public string $name = "x";
来源：http://gkw.chenjidiqi.icu

JS:   this.name = "x";
来源：http://guo.xinyue.icu

TS:   name: string = "x";
来源：http://tjw.c1oappe.top

Java: private String name;
来源：http://pjp.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngw.pengpengdd.cyou

Ruby: @name = "x"
来源：http://yrw.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://nfi.nanxuanxn.top

[G04] 定义方法
来源：http://bwn.redwolf501.top

Py:   def greet(self): return self.name
来源：http://isk.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xuw.yonumen.top

JS:   greet() { return this.name; }
来源：http://ocr.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://qtg.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://nrg.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jux.yonumen.top

Ruby: def greet; @name; end
来源：http://zzs.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://dxn.andypj.xyz

[G05] 继承
来源：http://wme.wangdashe.top

Py:   class Admin(User): pass
来源：http://wak.fengsongda.top

PHP:  class Admin extends User {}
来源：http://oft.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://gta.smart0.xyz

TS:   class Admin extends User {}
来源：http://mev.gaohongyu789.top

Java: class Admin extends User {}
来源：http://rzc.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mea.jinqigufen.top

Ruby: class Admin < User; end
来源：http://fpx.ydjk.org.cn

C#:   class Admin : User {}
来源：http://bvb.xziqi.cn


<!-- 参考信息 -->