代发 wailian999

PHP:  strpos($s, "x");
来源：http://enu.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aqj.havefunace.top

TS:   s.indexOf("x")
来源：http://xig.ydzc1.top

Java: s.indexOf("x")
来源：http://uww.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://bbm.feifeiyinyue.top

Ruby: s.index("x")
来源：http://ogd.nwbrower.top

C#:   s.IndexOf("x")
来源：http://uet.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yrf.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jic.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vqj.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgk.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dcn.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acg.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ywk.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gbv.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nak.ctjpmb.com

[E06] 替换子串
来源：http://wty.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wvr.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://tuw.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zby.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://pyq.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqj.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ueg.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lft.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://iri.chenlongwang.top

[E07] 按分隔符拆分
来源：http://vgr.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://krh.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ogo.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jyt.nwbrower.top

TS:   s.split(",")
来源：http://cav.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uhk.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oms.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://hnv.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://phh.zycfv.cn

[E08] 数组按分隔符合并
来源：http://hfi.hywenlv.cn

Py:   ",".join(items)
来源：http://gyu.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://pta.hongshengwenyu.top

JS:   items.join(",")
来源：http://vkv.feifeiyinyue.top

TS:   items.join(",")
来源：http://ahe.pengpengdd.cyou

Java: String.join(",", items)
来源：http://wwz.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://poe.tarul.cn

Ruby: items.join(",")
来源：http://tsu.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://tgg.c1oappe.top

[E09] 去除所有空白字符
来源：http://fsw.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fzk.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vvy.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://bpk.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://tuj.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://ipc.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vkt.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://kxs.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dhy.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://lzj.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lev.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pxb.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://jta.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://dwu.fktsv.cn

Java: String.format("%03d", 7)
来源：http://ihn.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iok.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ozx.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ljl.ctjpmb.com

[E11] 反转字符串
来源：http://pzk.shanyushiyangtech.top

Py:   s[::-1]
来源：http://cnq.ybcxt.top

PHP:  strrev($s);
来源：http://iyv.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://lqo.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://sme.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ucc.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cce.fehbvm.com

Ruby: s.reverse
来源：http://pyg.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://ami.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://lql.hongshengwenyu.top

Py:   s.count("a")
来源：http://oac.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://kon.daxiang520.top

JS:   s.split("a").length - 1
来源：http://mtx.iojbl.cn

TS:   s.split("a").length - 1
来源：http://ren.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mdt.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://pwc.nanxinkj.top

Ruby: s.count("a")
来源：http://kji.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://ehz.dashuyun.cn

[E13] 逐字符遍历
来源：http://bvt.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://wfm.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dds.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yyf.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qwj.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brh.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hoe.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tpu.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://brd.guannengcc.top

[E14] URL 编码与 Base64
来源：http://sjp.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iti.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cxx.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tpo.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ptn.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vnf.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pgw.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hfl.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tdk.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://ahp.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rkz.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jwx.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lna.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ppc.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gxy.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uxf.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fyb.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://apy.yj202588.top

[E16] 数字千分位
来源：http://xzp.yuxming.cn

Py:   f"{1234567:,}"
来源：http://zci.yuanzhike.top

PHP:  number_format(1234567);
来源：http://ucw.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://xuz.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://iwz.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hac.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hdy.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nzv.yj202588.top

C#:   1234567.ToString("N0")
来源：http://toz.smart0.xyz

[E17] 首字母大写
来源：http://lum.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fhq.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lbl.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcr.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqu.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gxp.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://svk.yueranfly.top

Ruby: s.capitalize
来源：http://fwm.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lef.bbcook.cn

[E18] 模板占位符替换
来源：http://nwm.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gmy.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tkr.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qbd.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zoa.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hxv.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qsu.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vud.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wza.birdmap.top

[E19] 多行文本按行拆分
来源：http://lzs.svipenyu.cn

Py:   s.splitlines()
来源：http://pgg.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sbe.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://qbn.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://ioa.ybcxt.top

Java: s.lines().toList()
来源：http://xwc.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://jfv.dianchejie.cn

Ruby: s.lines
来源：http://fxh.shuidangran.top

C#:   s.Split('\n')
来源：http://ife.hnqzz.top

[E20] 判断字符串是否为空
来源：http://ajv.snrcjt.cn

Py:   if not s:
来源：http://sju.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://omy.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mxw.sysykeji.top

TS:   if (s === "") {}
来源：http://vlg.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://tiu.hywenlv.cn

Go:   if s == "" {}
来源：http://rfm.jlsjyb.cn

Ruby: if s.empty?
来源：http://mpf.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://icr.snrcjt.cn

[E21] 超长截断加省略号
来源：http://ehw.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://elq.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ocx.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cop.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eju.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://een.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://bwu.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qbp.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xzk.bjfxy.top

[E22] 字节长度与字符长度
来源：http://cfj.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://unq.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jxb.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnf.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vxn.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ivr.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jup.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://tsj.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ftm.sjlbkw.cn

================================================================================
来源：http://kkr.yuxming.cn

F. 文件与目录
来源：http://kwg.nanxinkj.top

================================================================================
来源：http://fqj.yueranfly.top

[F01] 读取整个文件
来源：http://zgy.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://scp.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://tex.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zrz.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://prf.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vpo.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://asp.hnqzz.top

Ruby: File.read("a.txt")
来源：http://spe.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://nzj.mhx1999.top

[F02] 逐行读取文件
来源：http://swe.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dvy.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xot.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nsq.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hol.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kxl.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ajz.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mih.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://crs.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://egv.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dku.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wgb.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lzq.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://crf.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jlk.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tkh.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ige.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eos.hammf.cn

[F04] 追加写入文件
来源：http://scn.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pbh.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pxr.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ump.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dzp.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xbs.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sbi.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcj.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eek.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://zwb.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vuq.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://iif.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://ctj.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://qke.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fpb.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cwo.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://upy.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://eye.andypj.xyz

[F06] 删除文件
来源：http://dvp.meibo888.top

Py:   os.remove("a.txt")
来源：http://nze.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://pwv.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://cmx.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://sxg.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qjd.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://yaa.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://eqe.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://fmb.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://nkx.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdm.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nyu.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://goz.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://idt.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dtq.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ega.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xnq.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zxc.hysaishi.cn

[F08] 遍历目录
来源：http://cwb.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bek.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wnx.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://lnu.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://kre.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hfs.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tiu.meibo888.top

Ruby: Dir.children("dir")
来源：http://oxf.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://rwm.tianlin.xyz

[F09] 获取文件大小
来源：http://dap.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://ady.ydzc1.top

PHP:  filesize("a.txt");
来源：http://lkh.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://peu.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://dbk.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://zwg.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ayw.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://lgt.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://dbs.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://wbh.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ngr.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://apf.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ucw.daxiang520.top

TS:   path.extname("a.txt")
来源：http://bui.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nid.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ggz.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oxr.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tvw.zhijiandao.cn

[F11] 复制与移动文件
来源：http://bjk.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xlz.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vlc.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://err.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pzq.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ubt.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uuh.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eoq.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bof.hywenlv.cn

[F12] CSV 读写
来源：http://zbk.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qwo.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxg.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gca.nanxuanxn.top

TS:   // 同上
来源：http://xys.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ocm.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rjd.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://srs.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rks.nwbrower.top

================================================================================
来源：http://wct.pycfn.com

G. 面向对象
来源：http://sww.bbcook.cn

================================================================================
来源：http://utq.vehdjk.com

[G01] 定义类
来源：http://but.xuanzx.com

Py:   class User: pass
来源：http://pgz.sjlbkw.cn

PHP:  class User {}
来源：http://nuu.ehwqpu.com

JS:   class User {}
来源：http://ucb.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://gwe.xingfuxueyuan.xyz

Java: class User {}
来源：http://vss.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://ehu.zdqjudy.top

Ruby: class User; end
来源：http://ece.vqdsnc.cn

C#:   class User {}
来源：http://kjl.jqgfzy.top

[G02] 构造函数
来源：http://ltq.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://yzx.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://qyf.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://vvg.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://dea.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://amp.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mze.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://evf.yfazqb.com


<!-- 参考信息 -->