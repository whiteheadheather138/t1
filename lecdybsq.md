代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://bqz.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bja.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xor.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xpn.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://rhk.havefunace.top

[E07] 按分隔符拆分
来源：http://pos.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lcu.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mfz.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dit.xuanzx.com

TS:   s.split(",")
来源：http://kcc.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://fcr.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sor.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://rfl.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rgh.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://jhf.xinyue.icu

Py:   ",".join(items)
来源：http://yca.xylfe.cn

PHP:  implode(",", $items);
来源：http://hts.jlsjyb.cn

JS:   items.join(",")
来源：http://zrf.chenjidiqi.icu

TS:   items.join(",")
来源：http://xsq.hcnkem.com

Java: String.join(",", items)
来源：http://hpx.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://uhf.ppjwa.cn

Ruby: items.join(",")
来源：http://gjh.andypj.xyz

C#:   string.Join(",", items)
来源：http://ikn.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://wsn.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xck.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fuu.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://wrk.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://adi.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://mds.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://whd.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://chi.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mfq.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://aev.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kbu.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://puc.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://qpb.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://jkj.mhx1999.top

Java: String.format("%03d", 7)
来源：http://yji.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wve.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://alj.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qoj.snrcjt.cn

[E11] 反转字符串
来源：http://yzq.feifeiyinyue.top

Py:   s[::-1]
来源：http://kfk.hnxiangtu.top

PHP:  strrev($s);
来源：http://etk.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://tfa.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://jdr.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lsq.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmm.gaohongyu789.top

Ruby: s.reverse
来源：http://gfb.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://wzw.hcnkem.com

[E12] 统计某字符出现次数
来源：http://jev.birdmap.top

Py:   s.count("a")
来源：http://mkn.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://zuk.uphjek.com

JS:   s.split("a").length - 1
来源：http://mbl.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://hey.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pqa.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://jrf.cqqwz.cn

Ruby: s.count("a")
来源：http://fxt.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://nvl.zycfv.cn

[E13] 逐字符遍历
来源：http://xqx.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://zew.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bxs.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hns.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ifi.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dby.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qda.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qzv.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ywo.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://khj.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gux.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aun.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yaz.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yag.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ddb.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uuw.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yvd.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ozx.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://edd.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dxs.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nlt.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gca.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uqc.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xov.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ymj.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pyv.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vbj.yuxming.cn

[E16] 数字千分位
来源：http://vsh.meibo888.top

Py:   f"{1234567:,}"
来源：http://fel.iojbl.cn

PHP:  number_format(1234567);
来源：http://xit.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dcz.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://lir.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vey.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pst.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rau.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://gbj.vqdsnc.cn

[E17] 首字母大写
来源：http://fyi.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dji.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldt.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://moa.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ujb.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rtn.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qns.redwolf501.top

Ruby: s.capitalize
来源：http://dhk.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wzy.daxiang520.top

[E18] 模板占位符替换
来源：http://llv.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://evn.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qtn.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qul.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tpx.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gex.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kji.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ght.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rqb.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://hrm.tian-w.cn

Py:   s.splitlines()
来源：http://osp.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aej.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://pyy.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://kro.sxryk.cn

Java: s.lines().toList()
来源：http://bre.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://vxb.yj20258.top

Ruby: s.lines
来源：http://kyf.vqdsnc.cn

C#:   s.Split('\n')
来源：http://tyn.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://tes.fzhhl.top

Py:   if not s:
来源：http://aok.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbi.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tno.hesvh.cn

TS:   if (s === "") {}
来源：http://zod.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://uwt.cucudq.cn

Go:   if s == "" {}
来源：http://qkv.chenzaomai.com

Ruby: if s.empty?
来源：http://ywa.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zcn.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://mjo.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wys.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nuw.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pix.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://djh.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zld.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://zjb.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ote.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bci.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://hpf.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cqt.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxh.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blp.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bqw.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ntj.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vxh.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://lvv.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://apy.52xcode.cn

================================================================================
来源：http://ebz.zhoulong.xyz

F. 文件与目录
来源：http://rik.cheryme.top

================================================================================
来源：http://mmc.iojbl.cn

[F01] 读取整个文件
来源：http://qop.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vlf.meibo888.top

PHP:  file_get_contents("a.txt");
来源：http://bqv.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jcc.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oek.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://spb.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kah.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://nta.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://yqw.hysaishi.cn

[F02] 逐行读取文件
来源：http://rmn.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jvz.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://csr.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxe.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://asu.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ayl.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vny.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqz.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nnj.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://awj.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yxa.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tqe.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwk.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qin.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vul.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zmk.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://mqd.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bie.sufxvd.cn

[F04] 追加写入文件
来源：http://ejn.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vfd.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tsy.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oaw.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpq.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://krw.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tkb.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hou.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ost.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://ica.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://caf.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://tgc.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://swo.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://epg.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://znb.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dvz.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://ayv.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://wzx.smart0.xyz

[F06] 删除文件
来源：http://ikv.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://ltb.smart0.xyz

PHP:  unlink("a.txt");
来源：http://mnl.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rlr.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://fdu.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cuc.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://ztc.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://mdc.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://kbd.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://zlm.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pya.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ctj.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxx.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovg.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxp.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xon.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvp.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hwq.jinqigufen.top

[F08] 遍历目录
来源：http://toq.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hpu.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xti.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://zfv.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://ico.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pvm.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bnx.xziqi.cn

Ruby: Dir.children("dir")
来源：http://xts.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://egl.zhoulong.xyz

[F09] 获取文件大小
来源：http://jih.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://eoh.nwbrower.top

PHP:  filesize("a.txt");
来源：http://jrf.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://ewt.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://nxi.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://rnu.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sdf.aizwys.cn

Ruby: File.size("a.txt")
来源：http://blj.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://rpu.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://sir.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ebh.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rjz.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dpy.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://eyk.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mnl.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gde.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pei.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xjb.fktsv.cn

[F11] 复制与移动文件
来源：http://wtm.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://etd.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sjy.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tuv.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwc.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ehq.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jxd.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpp.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gpl.xinyue.icu

[F12] CSV 读写
来源：http://bed.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ckl.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bzp.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cky.jlsjyb.cn

TS:   // 同上
来源：http://evg.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ift.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kuu.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eqe.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sxx.hammf.cn

================================================================================
来源：http://cyt.bjfxy.top

G. 面向对象
来源：http://orr.vehdjk.com

================================================================================
来源：http://nrp.cashguo.top

[G01] 定义类
来源：http://iqy.sweek.top

Py:   class User: pass
来源：http://etf.jyoumei.cn

PHP:  class User {}
来源：http://vlt.jyoumei.cn

JS:   class User {}
来源：http://pbb.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://jpz.zhengqikj.top

Java: class User {}
来源：http://fks.yj20258.top

Go:   type User struct { Name string }
来源：http://lgk.cheryme.top

Ruby: class User; end
来源：http://fmb.hfpthk.cn

C#:   class User {}
来源：http://yey.jyoumei.cn

[G02] 构造函数
来源：http://knu.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wsr.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://tbc.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://ydm.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://mmy.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://amk.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rpi.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wqd.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://lge.vehdjk.com

[G03] 实例属性
来源：http://kke.yongpay.top

Py:   self.name = "x"
来源：http://qbz.tianlin.xyz

PHP:  public string $name = "x";
来源：http://hfo.ydzc1.top

JS:   this.name = "x";
来源：http://jdk.yj20258.top

TS:   name: string = "x";
来源：http://blt.ybcxt.top

Java: private String name;
来源：http://ldu.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hqf.tarul.cn

Ruby: @name = "x"
来源：http://hia.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://gko.0kj1m.cn

[G04] 定义方法
来源：http://epw.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://ejt.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wby.bbcook.cn

JS:   greet() { return this.name; }
来源：http://ioc.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://pig.yonumen.top

Java: String greet() { return name; }
来源：http://zpg.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://klp.guannengcc.top

Ruby: def greet; @name; end
来源：http://xdc.xuanzx.com

C#:   public string Greet() => Name;
来源：http://yle.jiagoushi.top

[G05] 继承
来源：http://kcw.nanxinkj.top


<!-- 参考信息 -->