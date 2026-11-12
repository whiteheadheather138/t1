代发 wailian999

[E06] 替换子串
来源：http://rwi.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kff.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://hjs.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvu.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://tuo.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kso.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jrl.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://znq.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://jfm.smart0.xyz

[E07] 按分隔符拆分
来源：http://ryp.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://alz.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yme.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://rhs.yongpay.top

TS:   s.split(",")
来源：http://cmw.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://gbh.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cfo.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://bri.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ukk.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://mid.wangdashe.top

Py:   ",".join(items)
来源：http://gxn.jyoumei.cn

PHP:  implode(",", $items);
来源：http://lsc.jqgfzy.top

JS:   items.join(",")
来源：http://prr.nanxinkj.top

TS:   items.join(",")
来源：http://iaa.hcnkem.com

Java: String.join(",", items)
来源：http://zeu.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://wrd.yueranfly.top

Ruby: items.join(",")
来源：http://jkm.dianchejie.cn

C#:   string.Join(",", items)
来源：http://bnr.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://duo.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gqt.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcu.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://fhf.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://nsu.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://vvw.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ayd.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://irn.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zed.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://alb.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://por.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qeh.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://kff.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://jyx.hcnkem.com

Java: String.format("%03d", 7)
来源：http://nhx.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zlo.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qvv.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qcl.yangfankeji.com

[E11] 反转字符串
来源：http://fhj.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://ypf.xylfe.cn

PHP:  strrev($s);
来源：http://dof.316326.xyz

JS:   [...s].reverse().join("")
来源：http://ufg.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://lfr.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fxo.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhv.zdqjudy.top

Ruby: s.reverse
来源：http://drx.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://efi.sxryk.cn

[E12] 统计某字符出现次数
来源：http://gyw.pycfn.com

Py:   s.count("a")
来源：http://aac.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://mok.tian-w.cn

JS:   s.split("a").length - 1
来源：http://aec.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://cqv.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rom.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://mbh.jqgufenzy.top

Ruby: s.count("a")
来源：http://epm.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://jdc.316326.xyz

[E13] 逐字符遍历
来源：http://ugp.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://gjp.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eoz.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://akn.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://rns.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmb.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cim.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ttw.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ero.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://zli.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aea.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yga.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eua.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jgl.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yxz.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bzz.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uax.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dsh.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://tfd.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pwy.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tvt.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sqg.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rwh.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vdr.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oun.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwj.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ets.dashuyun.cn

[E16] 数字千分位
来源：http://bct.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://wks.hammf.cn

PHP:  number_format(1234567);
来源：http://cay.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bjz.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kaq.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xyd.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bqf.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://utt.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://als.nanxuanxn.top

[E17] 首字母大写
来源：http://vmk.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://inp.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bfv.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cvj.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kwa.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qnj.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iwq.ivvv.top

Ruby: s.capitalize
来源：http://ltl.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gtp.jqgufenzy.top

[E18] 模板占位符替换
来源：http://pnb.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cky.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ncr.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://itp.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lmo.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ios.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vfg.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oxl.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://odt.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://ood.hammf.cn

Py:   s.splitlines()
来源：http://enb.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vmg.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://ntj.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://ldq.sysykeji.top

Java: s.lines().toList()
来源：http://tom.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://tim.xuanzx.com

Ruby: s.lines
来源：http://cln.snrcjt.cn

C#:   s.Split('\n')
来源：http://hlo.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://drf.chenlongwang.top

Py:   if not s:
来源：http://skp.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://crb.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rey.mhx1999.top

TS:   if (s === "") {}
来源：http://vjo.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://rvo.chenlongwang.top

Go:   if s == "" {}
来源：http://ifj.jqgufenzy.top

Ruby: if s.empty?
来源：http://rrr.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjf.meibo888.top

[E21] 超长截断加省略号
来源：http://hys.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iup.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jeh.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxo.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://swm.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpc.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://csj.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zbd.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iot.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://htd.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://frq.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qeg.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tot.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcc.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zyd.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gfd.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://ipx.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dcx.52xcode.cn

================================================================================
来源：http://ebq.fzhhl.top

F. 文件与目录
来源：http://kdf.fanxiaobao.xyz

================================================================================
来源：http://uvu.zhengqikj.top

[F01] 读取整个文件
来源：http://bob.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ell.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://rgl.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ihj.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tqq.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://khn.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hep.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://ofc.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://gov.xylfe.cn

[F02] 逐行读取文件
来源：http://gzu.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fac.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ori.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bes.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ljl.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jya.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pkc.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://btm.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oun.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://apn.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qzq.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qbk.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sti.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://soe.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xzx.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycc.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://nhd.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nud.yj20258888.top

[F04] 追加写入文件
来源：http://kxs.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vkm.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxv.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lkf.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgz.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xcb.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dgo.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nyj.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xbw.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://oei.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tcp.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://sgm.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://tvx.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://tpa.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tyw.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tdp.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://nty.hammf.cn

C#:   File.Exists("a.txt")
来源：http://vqg.yj20258.top

[F06] 删除文件
来源：http://msl.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://yxs.ivvv.top

PHP:  unlink("a.txt");
来源：http://gzl.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://wfs.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ziu.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujm.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://tck.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://nwb.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://brj.nwbrower.top

[F07] 创建目录（含多级）
来源：http://vcd.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://umb.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uke.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bhs.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pii.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ara.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uku.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qaf.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aed.wangdashe.top

[F08] 遍历目录
来源：http://ldz.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ziy.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yek.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://dqa.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://xfz.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxi.andypj.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nkd.nwbrower.top

Ruby: Dir.children("dir")
来源：http://zig.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://qym.wangdashe.top

[F09] 获取文件大小
来源：http://jno.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://fwu.iojbl.cn

PHP:  filesize("a.txt");
来源：http://chn.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://bls.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://ssh.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://kcl.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mga.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://ehz.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://oft.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://ces.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mgd.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nvt.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://plb.iojbl.cn

TS:   path.extname("a.txt")
来源：http://wnd.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxr.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rjt.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fqo.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nac.ydzc1.top

[F11] 复制与移动文件
来源：http://moq.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jnv.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xpl.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpo.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lll.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sxh.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vnc.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kqt.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mea.yuxming.cn

[F12] CSV 读写
来源：http://iro.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cuu.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jdc.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byl.316326.xyz

TS:   // 同上
来源：http://ouy.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zvn.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://apa.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://htq.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://gxr.ctjpmb.com

================================================================================
来源：http://hbq.jqgfzy.top

G. 面向对象
来源：http://cho.316326.xyz

================================================================================
来源：http://ola.bbcook.cn

[G01] 定义类
来源：http://fwf.gzhubu.top

Py:   class User: pass
来源：http://lay.hammf.cn

PHP:  class User {}
来源：http://dsz.iojbl.cn

JS:   class User {}
来源：http://hki.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://klz.shangyingyoupin.top

Java: class User {}
来源：http://rsw.9152youxi.cn

Go:   type User struct { Name string }
来源：http://xks.cucudq.cn

Ruby: class User; end
来源：http://xhw.hammf.cn

C#:   class User {}
来源：http://hyv.zhixingplan.top

[G02] 构造函数
来源：http://vnp.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://obd.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://zwi.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://odh.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://gsv.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://hzg.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sig.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://qob.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://zou.fanxiaobao.xyz

[G03] 实例属性
来源：http://orm.daxiang520.top

Py:   self.name = "x"
来源：http://rce.yuxming.cn

PHP:  public string $name = "x";
来源：http://rtc.jiagoushi.top

JS:   this.name = "x";
来源：http://rer.yvedp.cn

TS:   name: string = "x";
来源：http://qys.vehdjk.com

Java: private String name;
来源：http://jso.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wjj.zdbjq.cn

Ruby: @name = "x"
来源：http://hdv.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://ffj.shanyushiyangkeji.top

[G04] 定义方法
来源：http://dso.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://bfv.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://cwu.yfazqb.com

JS:   greet() { return this.name; }
来源：http://nuz.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://dvn.ydjk.org.cn

Java: String greet() { return name; }
来源：http://ceb.sxryk.cn


<!-- 参考信息 -->