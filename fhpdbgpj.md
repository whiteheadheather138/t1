代发 wailian999

[E06] 替换子串
来源：http://oes.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cci.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://flc.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wwa.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://sui.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwz.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vcf.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xqz.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://vqk.gogol.net.cn

[E07] 按分隔符拆分
来源：http://iqk.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cpm.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nov.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dll.fzhhl.top

TS:   s.split(",")
来源：http://zao.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://gnh.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dhu.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://fsl.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://izm.yongpay.top

[E08] 数组按分隔符合并
来源：http://hzg.hywenlv.cn

Py:   ",".join(items)
来源：http://zrt.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://xsd.jinqigufen.top

JS:   items.join(",")
来源：http://wpu.dianchejie.cn

TS:   items.join(",")
来源：http://mon.52xcode.cn

Java: String.join(",", items)
来源：http://wpq.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://bmy.yfazqb.com

Ruby: items.join(",")
来源：http://dem.gotoacloud.top

C#:   string.Join(",", items)
来源：http://iws.yangfankeji.com

[E09] 去除所有空白字符
来源：http://dqg.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rxt.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kbm.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://vjf.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://yfs.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://dkk.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://ehp.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://tcb.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nxm.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://rbu.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hxy.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xcj.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://pfb.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://jrt.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://dma.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tqa.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://szs.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://swr.tian-w.cn

[E11] 反转字符串
来源：http://xey.ppjwa.cn

Py:   s[::-1]
来源：http://vrw.mhx1999.top

PHP:  strrev($s);
来源：http://whi.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://tpq.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://ypv.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yqj.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wlh.sysykeji.top

Ruby: s.reverse
来源：http://iap.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://nzz.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://wwz.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://khj.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://saw.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://oid.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://hsx.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://akk.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://bck.jqgfzy.top

Ruby: s.count("a")
来源：http://ubx.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://yaa.fehbvm.com

[E13] 逐字符遍历
来源：http://mct.sweek.top

Py:   for ch in s: print(ch)
来源：http://jtr.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bfz.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bvj.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://dey.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qny.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dxo.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://yzv.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dyw.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://rvh.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xyw.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bfv.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dkz.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhz.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ity.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pqz.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rai.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mfo.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://iwd.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://azs.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lcr.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wnx.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mml.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vdz.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xua.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cih.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hpb.0kj1m.cn

[E16] 数字千分位
来源：http://rfh.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://cxy.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://lph.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://efh.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jkl.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nkz.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oes.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rzt.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://nye.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://jek.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vvw.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ecq.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vtf.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yek.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wbl.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zou.birdmap.top

Ruby: s.capitalize
来源：http://sob.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lfd.cheryme.top

[E18] 模板占位符替换
来源：http://ury.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bau.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aob.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://woc.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nxr.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xni.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://azf.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dty.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wwk.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ydk.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://nrd.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gzx.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://yza.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://bbx.smart0.xyz

Java: s.lines().toList()
来源：http://ojh.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://ivf.52xcode.cn

Ruby: s.lines
来源：http://tte.quarkkingdee.top

C#:   s.Split('\n')
来源：http://doj.yfazqb.com

[E20] 判断字符串是否为空
来源：http://tlm.bjfxy.top

Py:   if not s:
来源：http://hfe.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cga.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfp.tian-w.cn

TS:   if (s === "") {}
来源：http://pcn.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://pqx.gzhubu.top

Go:   if s == "" {}
来源：http://emr.tarul.cn

Ruby: if s.empty?
来源：http://kar.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yxu.ivvv.top

[E21] 超长截断加省略号
来源：http://deb.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itv.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kxy.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ocb.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ecc.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blt.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://vjt.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pvz.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mcp.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://grh.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://olo.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynh.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://edm.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsa.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xcj.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yyy.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://jkw.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bft.jyoumei.cn

================================================================================
来源：http://yay.zhiwuduotai.top

F. 文件与目录
来源：http://ppj.dianchejie.cn

================================================================================
来源：http://uhh.zdqjudy.top

[F01] 读取整个文件
来源：http://gmv.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ebf.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://ggz.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://byo.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hqz.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jpp.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rgs.fengsongda.top

Ruby: File.read("a.txt")
来源：http://vgm.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://cll.hesvh.cn

[F02] 逐行读取文件
来源：http://wqk.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hai.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uuk.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fso.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nop.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qvd.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rpv.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aal.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pbr.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://inp.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://czs.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xvs.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tky.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vqu.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://krm.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lge.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://zav.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://scl.yj202588.top

[F04] 追加写入文件
来源：http://eiz.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ptg.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ths.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zur.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blo.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qxq.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fow.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gwx.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fvu.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://nkk.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wvt.meibo888.top

PHP:  file_exists("a.txt");
来源：http://kfz.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://zsx.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://vby.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kul.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ttu.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://fpt.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://tta.zhixingplan.top

[F06] 删除文件
来源：http://ihd.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://bwl.sweek.top

PHP:  unlink("a.txt");
来源：http://lbx.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gxc.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pav.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sjz.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://lps.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://byk.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://bxg.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://bae.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hlk.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dbh.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aaj.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bga.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ilp.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uel.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gbo.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zeg.guowangkeji.top

[F08] 遍历目录
来源：http://wyt.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kui.svipenyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pjv.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://ukx.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://nqi.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ipx.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://apm.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://lxf.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://hle.xziqi.cn

[F09] 获取文件大小
来源：http://ahd.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://jmq.guannengcc.top

PHP:  filesize("a.txt");
来源：http://xup.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://vvg.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://dgt.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://two.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://loe.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://vbx.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://dlk.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://vqf.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://skb.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cio.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hcp.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://lma.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ytx.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://anv.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ril.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://swd.haohaochexian.top

[F11] 复制与移动文件
来源：http://wep.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gmi.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vvd.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqc.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eth.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qrk.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmx.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fwd.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iza.yonumen.top

[F12] CSV 读写
来源：http://yzj.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://atr.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gpw.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ptz.52xcode.cn

TS:   // 同上
来源：http://pgd.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://frh.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ezd.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ioy.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://och.fzhhl.top

================================================================================
来源：http://vlw.haohaochexian.top

G. 面向对象
来源：http://dyt.aizwys.cn

================================================================================
来源：http://fdm.tanke756.top

[G01] 定义类
来源：http://unf.nwbrower.top

Py:   class User: pass
来源：http://myr.xylfe.cn

PHP:  class User {}
来源：http://rmb.shzxlz.cn

JS:   class User {}
来源：http://bbd.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://pod.guannengcc.top

Java: class User {}
来源：http://mcg.smart0.xyz

Go:   type User struct { Name string }
来源：http://wht.jinghuilouyu.cn

Ruby: class User; end
来源：http://akb.meibo888.top

C#:   class User {}
来源：http://qqk.haohaochexian.top

[G02] 构造函数
来源：http://grt.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ztj.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://pjt.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://fzz.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://ljw.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://upf.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eph.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://mlg.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://ngw.wangshuangyany.cn

[G03] 实例属性
来源：http://xnd.svipenyu.cn

Py:   self.name = "x"
来源：http://dvf.fehbvm.com

PHP:  public string $name = "x";
来源：http://oag.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://srs.cqqwz.cn

TS:   name: string = "x";
来源：http://xja.chenzaomai.com

Java: private String name;
来源：http://cfq.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rig.316326.xyz

Ruby: @name = "x"
来源：http://oxa.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://dkz.sweek.top

[G04] 定义方法
来源：http://bjp.fzhhl.top

Py:   def greet(self): return self.name
来源：http://nvt.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cjk.smart0.xyz

JS:   greet() { return this.name; }
来源：http://exi.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://iwo.jlsjyb.cn

Java: String greet() { return name; }
来源：http://yyl.tarul.cn


<!-- 参考信息 -->