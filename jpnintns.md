代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hit.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fvl.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ria.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bzu.feifeiyinyue.top

[E06] 替换子串
来源：http://ukd.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kvm.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://icf.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovx.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://kbz.52xcode.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gcg.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sja.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mpt.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://bvd.ehwqpu.com

[E07] 按分隔符拆分
来源：http://cux.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wri.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uqb.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mal.ehwqpu.com

TS:   s.split(",")
来源：http://wvb.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sxl.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qfq.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://jud.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://osr.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://cmk.gotoacloud.top

Py:   ",".join(items)
来源：http://vnw.tian-w.cn

PHP:  implode(",", $items);
来源：http://vsn.gotoacloud.top

JS:   items.join(",")
来源：http://vyi.yfazqb.com

TS:   items.join(",")
来源：http://rlp.gzhubu.top

Java: String.join(",", items)
来源：http://rki.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://jdv.yuxming.cn

Ruby: items.join(",")
来源：http://wra.52xcode.cn

C#:   string.Join(",", items)
来源：http://apg.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://orr.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yvp.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nkq.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://hmi.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://fsv.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://zog.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gta.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://abn.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://epc.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://vmu.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ocx.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://koi.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://lek.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://hxv.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://lhw.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ssi.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kim.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://efh.hywenlv.cn

[E11] 反转字符串
来源：http://aci.jinqigfzy.top

Py:   s[::-1]
来源：http://peg.fengsongda.top

PHP:  strrev($s);
来源：http://bzh.meibo888.top

JS:   [...s].reverse().join("")
来源：http://fzw.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://ixw.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dxi.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ysy.zhengqikj.top

Ruby: s.reverse
来源：http://svg.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://jyx.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://vwb.9152youxi.cn

Py:   s.count("a")
来源：http://yyn.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://kme.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://ofd.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://mqh.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gon.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://rxm.cdnleiting.top

Ruby: s.count("a")
来源：http://vcv.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://rfr.guannengcc.top

[E13] 逐字符遍历
来源：http://nis.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://qpj.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://crq.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ooo.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://noi.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nkd.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vee.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zid.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zfr.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://ybm.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kwx.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zmq.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zml.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://emg.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zqo.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kes.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwy.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yka.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://nir.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://syd.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://arf.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eqb.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ptv.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mjt.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxs.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ysn.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oqg.yvedp.cn

[E16] 数字千分位
来源：http://ckf.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://wtn.52xcode.cn

PHP:  number_format(1234567);
来源：http://zje.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jey.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wso.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kja.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gxw.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bql.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://iih.hnxiangtu.top

[E17] 首字母大写
来源：http://dpe.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbb.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zbr.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxi.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfu.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yyy.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ipj.dashuyun.cn

Ruby: s.capitalize
来源：http://udf.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ogg.xinyue.icu

[E18] 模板占位符替换
来源：http://ypj.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hpp.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://udh.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cjb.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://shu.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xqg.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zsn.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hfz.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cto.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://iso.guannengcc.top

Py:   s.splitlines()
来源：http://awh.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://idq.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://fyc.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://bls.sweek.top

Java: s.lines().toList()
来源：http://maq.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://awp.kuanghao11.cn

Ruby: s.lines
来源：http://yhc.yfazqb.com

C#:   s.Split('\n')
来源：http://nep.hammf.cn

[E20] 判断字符串是否为空
来源：http://voh.jinghuilouyu.cn

Py:   if not s:
来源：http://mpv.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lij.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxw.jianghu66.top

TS:   if (s === "") {}
来源：http://klf.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://xpo.snrcjt.cn

Go:   if s == "" {}
来源：http://aey.hcnkem.com

Ruby: if s.empty?
来源：http://cqv.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ahe.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://vml.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://diz.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jjw.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://frh.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trf.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kis.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://ibx.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wyv.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kyv.yuxming.cn

[E22] 字节长度与字符长度
来源：http://gcs.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pmo.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lxz.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://djn.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://muu.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gaa.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ybp.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://ych.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qvu.yj20258888.top

================================================================================
来源：http://zlc.hammf.cn

F. 文件与目录
来源：http://hmm.ppjwa.cn

================================================================================
来源：http://egb.yj20258.top

[F01] 读取整个文件
来源：http://hue.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jav.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://msi.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wxs.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://olg.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ahb.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ide.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://api.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://aea.gzhubu.top

[F02] 逐行读取文件
来源：http://sdo.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oqo.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yoc.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zzf.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgf.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wsi.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://evs.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://guv.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ygd.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://iuh.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cjj.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rcx.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dic.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://was.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ihs.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cwt.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://non.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://asp.ppjwa.cn

[F04] 追加写入文件
来源：http://xnw.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lcm.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://grs.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ftn.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsq.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dlp.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eej.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wdg.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rae.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://mcr.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kgb.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://ego.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://whn.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://whm.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nzd.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tnm.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://fpg.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://cgu.ydjk.org.cn

[F06] 删除文件
来源：http://imd.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://vxd.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://xbf.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://dkt.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oqp.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vur.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://qlb.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://frd.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://hyr.c1oappe.top

[F07] 创建目录（含多级）
来源：http://hco.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://syk.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ibu.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zib.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ali.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qpt.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://skb.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gmk.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://llm.cqqwz.cn

[F08] 遍历目录
来源：http://wwj.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oig.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lkv.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://emu.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://moo.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bvj.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yjg.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://kxc.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://dwi.aizwys.cn

[F09] 获取文件大小
来源：http://thh.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://tcc.yj20258.top

PHP:  filesize("a.txt");
来源：http://ycm.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://akt.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://amg.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://ifx.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://urj.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://hla.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://idu.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ren.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://heu.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qbp.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tbe.c1oappe.top

TS:   path.extname("a.txt")
来源：http://xbz.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qtf.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://urq.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vrn.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gqz.mhx1999.top

[F11] 复制与移动文件
来源：http://azw.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vme.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jua.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aou.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpf.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rbw.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mfn.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hlw.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ruf.yueranfly.top

[F12] CSV 读写
来源：http://qgm.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qtj.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yxk.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojk.fengsongda.top

TS:   // 同上
来源：http://ydn.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ceo.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://inj.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wbm.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xrr.meibo888.top

================================================================================
来源：http://aql.xinyue.icu

G. 面向对象
来源：http://ahy.uphjek.com

================================================================================
来源：http://hxu.jqgfzy.top

[G01] 定义类
来源：http://ptd.9152youxi.cn

Py:   class User: pass
来源：http://hph.jinqigufen.top

PHP:  class User {}
来源：http://vul.nanxuanxn.top

JS:   class User {}
来源：http://cfm.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://tfl.dashuyun.cn

Java: class User {}
来源：http://lin.fehbvm.com

Go:   type User struct { Name string }
来源：http://txw.fengsongda.top

Ruby: class User; end
来源：http://fhe.zycfv.cn

C#:   class User {}
来源：http://nro.sweek.top

[G02] 构造函数
来源：http://jxs.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://bzb.wangshuangyany.cn

PHP:  public function __construct(public string $name) {}
来源：http://qyt.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://wwa.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://pte.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://aqj.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dus.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://xmq.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://vup.uphjek.com

[G03] 实例属性
来源：http://iou.hcnkem.com

Py:   self.name = "x"
来源：http://irs.guowangkeji.top

PHP:  public string $name = "x";
来源：http://qhm.ehwqpu.com

JS:   this.name = "x";
来源：http://pap.yonumen.top

TS:   name: string = "x";
来源：http://wng.ctjpmb.com

Java: private String name;
来源：http://gyi.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://srh.ivvv.top

Ruby: @name = "x"
来源：http://flo.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://sax.snrcjt.cn

[G04] 定义方法
来源：http://uqk.hcnkem.com

Py:   def greet(self): return self.name
来源：http://qtq.jyoumei.cn


<!-- 参考信息 -->