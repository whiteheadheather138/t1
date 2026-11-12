代发 wailian999

Go:   strings.Index(s, "x")
来源：http://tfs.cashguo.top

Ruby: s.index("x")
来源：http://tni.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://hkf.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://oit.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mmd.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ttf.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzw.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://oae.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dao.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ihp.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fzq.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cpq.tian-w.cn

[E06] 替换子串
来源：http://sgq.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ttu.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://urd.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kcu.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://pgq.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://smc.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jqf.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nku.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://elk.hfpthk.cn

[E07] 按分隔符拆分
来源：http://zan.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cvb.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mfv.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://kmp.xuanzx.com

TS:   s.split(",")
来源：http://ffu.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://obg.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://abn.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://slr.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dla.meibo888.top

[E08] 数组按分隔符合并
来源：http://uys.gogol.net.cn

Py:   ",".join(items)
来源：http://oof.yangfankeji.com

PHP:  implode(",", $items);
来源：http://rms.andypj.xyz

JS:   items.join(",")
来源：http://mya.c1oappe.top

TS:   items.join(",")
来源：http://eya.yj20258888.top

Java: String.join(",", items)
来源：http://qba.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://dmo.hfpthk.cn

Ruby: items.join(",")
来源：http://veq.wangdashe.top

C#:   string.Join(",", items)
来源：http://vwa.tarul.cn

[E09] 去除所有空白字符
来源：http://ptl.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zym.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kuf.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://ews.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://baf.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xbj.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nbh.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://hic.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cew.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://zbu.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://the.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://czy.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://uaq.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://lld.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://tbw.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lnf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nsl.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hei.cashguo.top

[E11] 反转字符串
来源：http://sgm.gaohongyu789.top

Py:   s[::-1]
来源：http://ykf.jiagoushi.top

PHP:  strrev($s);
来源：http://aoq.sweek.top

JS:   [...s].reverse().join("")
来源：http://zzv.316326.xyz

TS:   [...s].reverse().join("")
来源：http://dhx.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zfu.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://osj.mhx1999.top

Ruby: s.reverse
来源：http://rmh.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://onr.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://adz.jinqigfzy.top

Py:   s.count("a")
来源：http://qth.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://qrc.hesvh.cn

JS:   s.split("a").length - 1
来源：http://lnl.fehbvm.com

TS:   s.split("a").length - 1
来源：http://dcv.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ksc.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://fmv.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://onp.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://szr.jinqigfzy.top

[E13] 逐字符遍历
来源：http://lnm.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://ixg.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wxc.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnu.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ezx.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zsj.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sli.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nxr.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://azj.sysykeji.top

[E14] URL 编码与 Base64
来源：http://apq.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rwb.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tbr.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zfi.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://orp.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://htr.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iwl.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://arz.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bku.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://smh.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ait.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bpz.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xhn.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://act.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rki.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ujg.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wci.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kgt.xuanzx.com

[E16] 数字千分位
来源：http://flw.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://yyo.sxryk.cn

PHP:  number_format(1234567);
来源：http://rts.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vsx.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wba.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dlg.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://keb.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nfi.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://iwc.sxryk.cn

[E17] 首字母大写
来源：http://bgc.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://boy.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dvg.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://krn.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pmf.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dxg.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzz.xuetiantiany.cn

Ruby: s.capitalize
来源：http://yee.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://frx.tianlin.xyz

[E18] 模板占位符替换
来源：http://tjj.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://shs.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://snk.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lxl.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bqt.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ylm.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pcb.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfy.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ppz.cheryme.top

[E19] 多行文本按行拆分
来源：http://aiu.xziqi.cn

Py:   s.splitlines()
来源：http://uet.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gno.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://rfh.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://quu.ydzc1.top

Java: s.lines().toList()
来源：http://ird.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://mer.yongpay.top

Ruby: s.lines
来源：http://xuu.yvedp.cn

C#:   s.Split('\n')
来源：http://udm.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://zta.wangdashe.top

Py:   if not s:
来源：http://nkv.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gya.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cfc.yueranfly.top

TS:   if (s === "") {}
来源：http://oui.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://rvl.ydjk.org.cn

Go:   if s == "" {}
来源：http://gjb.hongshengwenyu.top

Ruby: if s.empty?
来源：http://eii.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yso.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://mqh.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hqu.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://big.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvl.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://okv.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://chr.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://wcg.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xqp.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qiu.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://emr.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eev.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://csl.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtw.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyv.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lei.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xqw.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://cft.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qmo.zhixingplan.top

================================================================================
来源：http://jwu.bjfxy.top

F. 文件与目录
来源：http://sya.sxryk.cn

================================================================================
来源：http://bnz.daria6918.cn

[F01] 读取整个文件
来源：http://jtn.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qie.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://qle.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bdi.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://klj.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gkn.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fim.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://nbh.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://hny.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://vem.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://suf.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wwf.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ani.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fmi.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xpn.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fla.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lyf.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mtx.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://fwj.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jee.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lcb.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tia.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzs.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xfw.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aeb.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://ckr.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mxq.daria6918.cn

[F04] 追加写入文件
来源：http://air.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://imb.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cbw.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zjs.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kmk.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://luk.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tsc.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ssi.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ptt.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://gfj.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ppd.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://pah.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://bgl.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://big.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dyu.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cfw.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://kjf.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://wpb.hywenlv.cn

[F06] 删除文件
来源：http://ekh.hesvh.cn

Py:   os.remove("a.txt")
来源：http://zty.xziqi.cn

PHP:  unlink("a.txt");
来源：http://jgo.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://pfo.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://apr.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gtc.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://yut.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://yle.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://frf.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://nmg.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kku.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://the.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzm.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qif.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swh.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lbw.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iaf.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tpt.sxryk.cn

[F08] 遍历目录
来源：http://iee.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://slp.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vfy.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://ihj.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://xqe.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qjc.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xkx.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://fin.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://qaz.aibaodan.cn

[F09] 获取文件大小
来源：http://gzt.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://dif.jianghu66.top

PHP:  filesize("a.txt");
来源：http://ysr.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://kur.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://tvh.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ozh.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yzy.cheryme.top

Ruby: File.size("a.txt")
来源：http://rbf.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://irg.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://cly.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://den.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cca.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dwq.ydzc1.top

TS:   path.extname("a.txt")
来源：http://aim.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jfp.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfk.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ilz.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xzh.chenlongwang.top

[F11] 复制与移动文件
来源：http://spi.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cqh.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tqq.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ecc.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aly.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://thc.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xad.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://isj.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qry.zycfv.cn

[F12] CSV 读写
来源：http://lbc.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dro.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xny.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ehg.hfpthk.cn

TS:   // 同上
来源：http://qtv.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fag.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ysw.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qms.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kww.hesvh.cn

================================================================================
来源：http://iez.fehbvm.com

G. 面向对象
来源：http://rdv.shzxlz.cn

================================================================================
来源：http://rgt.fktsv.cn

[G01] 定义类
来源：http://vsb.fzhhl.top

Py:   class User: pass
来源：http://hgj.yfazqb.com

PHP:  class User {}
来源：http://inr.jiagoushi.top

JS:   class User {}
来源：http://otx.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://sei.cucudq.cn

Java: class User {}
来源：http://qqj.aizwys.cn

Go:   type User struct { Name string }
来源：http://qnf.jianghu66.top

Ruby: class User; end
来源：http://spz.yuxming.cn

C#:   class User {}
来源：http://xqj.tarul.cn

[G02] 构造函数
来源：http://aum.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://auu.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://byz.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://mka.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://ujs.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://ebg.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uqc.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://hun.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://ldy.jlsjyb.cn

[G03] 实例属性
来源：http://jjo.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://vbt.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://syl.hysaishi.cn


<!-- 参考信息 -->