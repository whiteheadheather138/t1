代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gtw.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vrr.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mlu.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://roo.jinqigufen.top

[E06] 替换子串
来源：http://kdp.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zqj.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ori.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hui.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://nux.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hav.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pnl.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rfl.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://nun.sxryk.cn

[E07] 按分隔符拆分
来源：http://whx.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://twv.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zcx.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xff.sufxvd.cn

TS:   s.split(",")
来源：http://yih.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://mbk.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://exm.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://yug.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xei.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://rwk.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://qja.nwbrower.top

PHP:  implode(",", $items);
来源：http://lxd.cheryme.top

JS:   items.join(",")
来源：http://gaa.sjlbkw.cn

TS:   items.join(",")
来源：http://fgw.fehbvm.com

Java: String.join(",", items)
来源：http://yoa.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://vwk.hnxiangtu.top

Ruby: items.join(",")
来源：http://mmf.jqgfzy.top

C#:   string.Join(",", items)
来源：http://aiy.daria6918.cn

[E09] 去除所有空白字符
来源：http://igg.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rad.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpu.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://hku.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://nuu.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://iui.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://wha.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jmc.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://htg.fehbvm.com

[E10] 左侧补零 / 定长填充
来源：http://nmh.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ell.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xpz.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://awi.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://vdz.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://hjy.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ovx.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://djv.cheryme.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ucr.yanxiufei.cn

[E11] 反转字符串
来源：http://zqz.zdbjq.cn

Py:   s[::-1]
来源：http://wtf.shzxlz.cn

PHP:  strrev($s);
来源：http://ngh.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://uyp.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://ytb.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://rlr.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://msr.xylfe.cn

Ruby: s.reverse
来源：http://ytg.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ymg.xylfe.cn

[E12] 统计某字符出现次数
来源：http://tku.ybcxt.top

Py:   s.count("a")
来源：http://lrm.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://csu.iojbl.cn

JS:   s.split("a").length - 1
来源：http://new.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://kta.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lcr.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://aob.fengsongda.top

Ruby: s.count("a")
来源：http://tte.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://gui.fktsv.cn

[E13] 逐字符遍历
来源：http://fho.yj20258.top

Py:   for ch in s: print(ch)
来源：http://kim.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lax.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iue.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oqs.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://opa.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cib.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://inq.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhr.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://kle.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rsl.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rbm.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://det.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pzj.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ckd.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xwp.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kid.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swr.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://tkl.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gjb.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hon.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ayq.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jaq.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbq.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dze.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pkb.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wfi.cdnleiting.top

[E16] 数字千分位
来源：http://rmd.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://lvu.meibo888.top

PHP:  number_format(1234567);
来源：http://deh.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://shm.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hpd.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jkh.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://idb.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kem.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://kip.gzhubu.top

[E17] 首字母大写
来源：http://iah.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ddz.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ocq.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjm.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfd.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyz.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nju.ctjpmb.com

Ruby: s.capitalize
来源：http://fjy.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://voa.jianghu66.top

[E18] 模板占位符替换
来源：http://fpd.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mrp.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bim.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uik.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ket.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jts.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://opo.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oaq.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xoi.316326.xyz

[E19] 多行文本按行拆分
来源：http://yoe.pengpengdd.cyou

Py:   s.splitlines()
来源：http://cok.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://usc.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://vaa.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://prw.redwolf501.top

Java: s.lines().toList()
来源：http://lqp.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://xcy.sweek.top

Ruby: s.lines
来源：http://oab.yj20258888.top

C#:   s.Split('\n')
来源：http://zfi.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://xtc.hywenlv.cn

Py:   if not s:
来源：http://wfx.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gzr.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://two.cdnleiting.top

TS:   if (s === "") {}
来源：http://oid.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://jnd.hfpthk.cn

Go:   if s == "" {}
来源：http://ide.xziqi.cn

Ruby: if s.empty?
来源：http://kmr.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://etr.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://vvw.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pur.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zyd.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfb.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxx.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ube.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://qly.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bin.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eex.yfazqb.com

[E22] 字节长度与字符长度
来源：http://mjh.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jgz.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fok.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxg.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkt.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://siy.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cot.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://kxe.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ihv.andypj.xyz

================================================================================
来源：http://dpt.jyoumei.cn

F. 文件与目录
来源：http://vcu.sjlbkw.cn

================================================================================
来源：http://vqm.iojbl.cn

[F01] 读取整个文件
来源：http://vzj.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hwi.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://gqy.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bch.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rax.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fnr.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://use.smart0.xyz

Ruby: File.read("a.txt")
来源：http://ymh.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://vpk.cashguo.top

[F02] 逐行读取文件
来源：http://jhy.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vcn.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rcd.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfq.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cez.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ueu.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ann.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tqd.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://juc.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://bdr.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gei.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dhx.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxy.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://scq.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zdg.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xwk.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://qks.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mnh.svipenyu.cn

[F04] 追加写入文件
来源：http://bze.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mrr.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kow.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aab.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pjb.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iak.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xav.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wxs.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vgi.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://zxh.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bnp.tarul.cn

PHP:  file_exists("a.txt");
来源：http://bgi.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://fbt.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://gil.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ttv.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hss.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://nke.yj202588.top

C#:   File.Exists("a.txt")
来源：http://bgp.quarkkingdee.top

[F06] 删除文件
来源：http://kpt.vehdjk.com

Py:   os.remove("a.txt")
来源：http://igy.shuidangran.top

PHP:  unlink("a.txt");
来源：http://nbu.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://nod.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bni.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://alj.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://tbc.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://svg.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://aym.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://ylu.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oug.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://klz.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iwy.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwp.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hsi.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yip.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yeg.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://twv.chenlongwang.top

[F08] 遍历目录
来源：http://puf.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://srx.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tti.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://aui.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://vvs.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tzz.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://hob.sxryk.cn

Ruby: Dir.children("dir")
来源：http://xkd.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://zky.cqqwz.cn

[F09] 获取文件大小
来源：http://smx.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://upf.xylfe.cn

PHP:  filesize("a.txt");
来源：http://cay.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://gvv.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://wnj.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://sta.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://plw.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://gqx.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://udo.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ade.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mhp.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zkn.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ptl.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://pel.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qli.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rik.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hpb.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hxg.zhijiandao.cn

[F11] 复制与移动文件
来源：http://ydb.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://huc.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nzh.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rih.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jdu.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nvw.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fal.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dat.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oee.wangdashe.top

[F12] CSV 读写
来源：http://lxu.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wsg.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://joz.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://veq.tianlin.xyz

TS:   // 同上
来源：http://qxg.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vyc.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://akl.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eby.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ocd.jyoumei.cn

================================================================================
来源：http://hlx.guannengcc.top

G. 面向对象
来源：http://gzb.jianghu66.top

================================================================================
来源：http://mck.dianchejie.cn

[G01] 定义类
来源：http://vrs.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://ldc.fktsv.cn

PHP:  class User {}
来源：http://fgj.gaohongyu789.top

JS:   class User {}
来源：http://asz.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://pko.ybcxt.top

Java: class User {}
来源：http://nkl.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://vhx.c1oappe.top

Ruby: class User; end
来源：http://tkl.nanxuanxn.top

C#:   class User {}
来源：http://nxb.yj20258.top

[G02] 构造函数
来源：http://zpc.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://qta.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://tty.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://avq.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://nnb.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://xcp.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tjb.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://nwf.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://qjm.cashguo.top

[G03] 实例属性
来源：http://nut.tianlin.xyz

Py:   self.name = "x"
来源：http://iin.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://gbz.guannengcc.top

JS:   this.name = "x";
来源：http://xgr.hongshengwenyu.top

TS:   name: string = "x";
来源：http://bao.sweek.top

Java: private String name;
来源：http://sxd.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qia.dashuyun.cn

Ruby: @name = "x"
来源：http://idx.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jid.chenzaomai.com

[G04] 定义方法
来源：http://bii.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://duw.zycfv.cn


<!-- 参考信息 -->