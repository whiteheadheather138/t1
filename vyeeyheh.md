代发 wailian999

[E06] 替换子串
来源：http://hjl.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dqr.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://crz.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txr.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://qbn.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nsy.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yra.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vys.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://fjf.mhx1999.top

[E07] 按分隔符拆分
来源：http://ewu.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://icx.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ixv.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dih.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://nlb.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://cmf.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wcx.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://xhm.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aim.sxryk.cn

[E08] 数组按分隔符合并
来源：http://ufg.0kj1m.cn

Py:   ",".join(items)
来源：http://lcr.zdqjudy.top

PHP:  implode(",", $items);
来源：http://wlr.c1oappe.top

JS:   items.join(",")
来源：http://txc.nwbrower.top

TS:   items.join(",")
来源：http://hyh.ydzc1.top

Java: String.join(",", items)
来源：http://mzm.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://zuu.yanxiufei.cn

Ruby: items.join(",")
来源：http://tbq.shzxlz.cn

C#:   string.Join(",", items)
来源：http://gjg.yongpay.top

[E09] 去除所有空白字符
来源：http://dxs.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pmv.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gyc.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://lzz.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://yrv.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://ooy.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qct.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://rji.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bdo.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://ntu.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jes.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mog.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://jnj.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://cor.yvedp.cn

Java: String.format("%03d", 7)
来源：http://llj.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lfg.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kyw.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vdj.cashguo.top

[E11] 反转字符串
来源：http://qlj.chenlongwang.top

Py:   s[::-1]
来源：http://lze.cashguo.top

PHP:  strrev($s);
来源：http://hxp.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://rzk.cheryme.top

TS:   [...s].reverse().join("")
来源：http://drc.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://cuc.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ngc.cashguo.top

Ruby: s.reverse
来源：http://jes.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://vbu.hesvh.cn

[E12] 统计某字符出现次数
来源：http://zsy.jqgfzy.top

Py:   s.count("a")
来源：http://lzu.yonumen.top

PHP:  substr_count($s, "a");
来源：http://ujl.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://mmp.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://ncx.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ema.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://rwu.guannengcc.top

Ruby: s.count("a")
来源：http://ioe.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://zhi.yanxiufei.cn

[E13] 逐字符遍历
来源：http://zww.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://cfq.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hym.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wim.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ikt.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://swa.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qpy.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nfj.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ihk.gzhubu.top

[E14] URL 编码与 Base64
来源：http://wfn.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dty.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tme.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bqq.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://slz.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fkn.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jcu.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mmw.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mtt.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://jtr.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://uqf.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ito.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xpd.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nym.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bbn.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tug.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vxx.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://umd.havefunace.top

[E16] 数字千分位
来源：http://elm.cashguo.top

Py:   f"{1234567:,}"
来源：http://vdz.fengsongda.top

PHP:  number_format(1234567);
来源：http://qgy.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ztg.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fnq.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rdn.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sgu.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cni.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://ejz.jqgufenzy.top

[E17] 首字母大写
来源：http://vna.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bkq.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://ujd.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xyl.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bwz.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lbm.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bbe.aizwys.cn

Ruby: s.capitalize
来源：http://zec.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pmq.fktsv.cn

[E18] 模板占位符替换
来源：http://nnq.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mor.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://njq.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://wag.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://agc.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qgy.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pxg.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://clb.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://znv.cucudq.cn

[E19] 多行文本按行拆分
来源：http://fxn.ctjpmb.com

Py:   s.splitlines()
来源：http://cor.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iqg.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://kii.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://pzb.zhoulong.xyz

Java: s.lines().toList()
来源：http://lar.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://fcb.jqgufenzy.top

Ruby: s.lines
来源：http://ofy.jinqigufen.top

C#:   s.Split('\n')
来源：http://oxw.ybcxt.top

[E20] 判断字符串是否为空
来源：http://zsb.jinghuilouyu.cn

Py:   if not s:
来源：http://clm.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uww.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fmr.dashuyun.cn

TS:   if (s === "") {}
来源：http://ocn.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://tse.ydjk.org.cn

Go:   if s == "" {}
来源：http://pev.bbcook.cn

Ruby: if s.empty?
来源：http://pqa.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zko.zhengqikj.top

[E21] 超长截断加省略号
来源：http://oyx.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jch.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fsg.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mms.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynj.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yjz.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://ads.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmy.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dcx.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://imz.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hip.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywt.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjo.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fll.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sfy.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bpo.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://dkf.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bpk.vqdsnc.cn

================================================================================
来源：http://jjd.uphjek.com

F. 文件与目录
来源：http://urp.snrcjt.cn

================================================================================
来源：http://drb.redwolf501.top

[F01] 读取整个文件
来源：http://avw.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://egr.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://sjc.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pmo.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://puu.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tej.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fqb.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://snt.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ugy.gogol.net.cn

[F02] 逐行读取文件
来源：http://flb.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rzm.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvz.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iuy.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yhm.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://htq.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://suh.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tpk.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vae.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://gio.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rde.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jim.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enq.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://phw.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zfi.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nue.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://sgh.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yyv.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://dql.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bux.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gcm.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpe.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsj.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xpe.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zzc.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zbq.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://shc.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://nqh.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yuy.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://xgj.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://tkp.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://iyh.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fss.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vau.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://yrd.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://wjn.gogol.net.cn

[F06] 删除文件
来源：http://zww.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://dxo.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://xhv.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xlt.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://akj.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eja.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://daw.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://vlp.tarul.cn

C#:   File.Delete("a.txt");
来源：http://ecf.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://vnn.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://big.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uzn.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aqx.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://epu.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fnv.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cqw.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mcc.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lpf.zycfv.cn

[F08] 遍历目录
来源：http://auj.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lwq.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vmy.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://nuo.sweek.top

TS:   fs.readdirSync("dir")
来源：http://gzq.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zhc.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cqs.daxiang520.top

Ruby: Dir.children("dir")
来源：http://xpa.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://rwj.haohaochexian.top

[F09] 获取文件大小
来源：http://fjp.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://fvf.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://nlb.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://fmk.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://pmp.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://smc.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rhx.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://amf.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://kfh.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://xxz.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wjh.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yxr.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqw.daria6918.cn

TS:   path.extname("a.txt")
来源：http://jdn.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wsi.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wuj.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://szx.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iva.shzxlz.cn

[F11] 复制与移动文件
来源：http://mdr.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gls.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqe.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdb.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zvm.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blz.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://msn.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qvz.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ncl.feifeiyinyue.top

[F12] CSV 读写
来源：http://sve.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ofc.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sxc.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qig.hysaishi.cn

TS:   // 同上
来源：http://rfp.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ikp.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://poz.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqx.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gsk.sufxvd.cn

================================================================================
来源：http://uyp.yueranfly.top

G. 面向对象
来源：http://fyv.xziqi.cn

================================================================================
来源：http://inx.yongpay.top

[G01] 定义类
来源：http://xqm.yangfankeji.com

Py:   class User: pass
来源：http://eva.hammf.cn

PHP:  class User {}
来源：http://jsk.cucudq.cn

JS:   class User {}
来源：http://vpe.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://avy.cucudq.cn

Java: class User {}
来源：http://bwr.ybcxt.top

Go:   type User struct { Name string }
来源：http://xsz.vqdsnc.cn

Ruby: class User; end
来源：http://ofe.hnxiangtu.top

C#:   class User {}
来源：http://egb.mhx1999.top

[G02] 构造函数
来源：http://rwm.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://fjp.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://uvq.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://ksd.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://yuh.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://dcy.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bsc.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://zgo.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://rub.yongpay.top

[G03] 实例属性
来源：http://yda.vqdsnc.cn

Py:   self.name = "x"
来源：http://ctv.yj20258888.top

PHP:  public string $name = "x";
来源：http://xrg.pycfn.com

JS:   this.name = "x";
来源：http://eah.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://slf.zhixingplan.top

Java: private String name;
来源：http://dlq.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hio.sufxvd.cn

Ruby: @name = "x"
来源：http://qea.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://wtk.nanxuanxn.top

[G04] 定义方法
来源：http://icf.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://srf.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hsj.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://ihw.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://adq.cucudq.cn

Java: String greet() { return name; }
来源：http://jmb.jianghu66.top


<!-- 参考信息 -->