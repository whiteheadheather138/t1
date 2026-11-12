代发 wailian999

[E06] 替换子串
来源：http://ffu.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qik.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://cwu.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tby.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://aob.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgl.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vxp.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jid.cheryme.top

C#:   s.Replace("a", "b")
来源：http://yyk.iojbl.cn

[E07] 按分隔符拆分
来源：http://yzp.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jzl.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xrk.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ukm.hesvh.cn

TS:   s.split(",")
来源：http://ukr.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mpq.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mjl.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://kdp.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://niv.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://bhn.yanxiufei.cn

Py:   ",".join(items)
来源：http://yyq.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://deg.fktsv.cn

JS:   items.join(",")
来源：http://qmc.jiagoushi.top

TS:   items.join(",")
来源：http://xqx.tarul.cn

Java: String.join(",", items)
来源：http://qpw.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://bru.tarul.cn

Ruby: items.join(",")
来源：http://rho.jinqigufen.top

C#:   string.Join(",", items)
来源：http://arx.316326.xyz

[E09] 去除所有空白字符
来源：http://xym.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tru.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dcg.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://opo.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://dqn.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://oyo.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zgm.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yjn.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lsb.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://ggr.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ovo.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://diz.sweek.top

JS:   "7".padStart(3, "0")
来源：http://qji.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://yoq.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://lmv.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://evg.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mya.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zhh.fzhhl.top

[E11] 反转字符串
来源：http://bhw.gaohongyu789.top

Py:   s[::-1]
来源：http://rgm.vqdsnc.cn

PHP:  strrev($s);
来源：http://caz.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://dfi.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://vxb.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nqs.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://byz.cqqwz.cn

Ruby: s.reverse
来源：http://jbg.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://ugd.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://tpt.chenzaomai.com

Py:   s.count("a")
来源：http://bmv.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://yvw.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://xrh.gzhubu.top

TS:   s.split("a").length - 1
来源：http://ynf.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://woi.hammf.cn

Go:   strings.Count(s, "a")
来源：http://tdx.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://qyx.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://vco.snrcjt.cn

[E13] 逐字符遍历
来源：http://hbl.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://nkw.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qbl.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gju.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://odg.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aey.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cpd.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aaf.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kgi.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://ofs.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://flv.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ksi.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://apu.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://plb.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vkd.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yax.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fah.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gnn.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://mxl.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dad.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://msr.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bfi.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://itg.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ahl.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ump.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ivn.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wwn.ybcxt.top

[E16] 数字千分位
来源：http://hvc.nwbrower.top

Py:   f"{1234567:,}"
来源：http://ydj.hywenlv.cn

PHP:  number_format(1234567);
来源：http://rso.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mvv.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xem.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hif.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fak.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ryy.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://ymm.uphjek.com

[E17] 首字母大写
来源：http://jyn.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgr.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kgs.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qee.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbi.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ura.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aew.sysykeji.top

Ruby: s.capitalize
来源：http://lgd.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xjm.fengsongda.top

[E18] 模板占位符替换
来源：http://rjx.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ysz.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gbm.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jiu.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jqd.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fkj.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ryt.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dpl.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bzt.cucudq.cn

[E19] 多行文本按行拆分
来源：http://tem.hysaishi.cn

Py:   s.splitlines()
来源：http://uph.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://byd.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://cfd.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://hta.quarkkingdee.top

Java: s.lines().toList()
来源：http://vmb.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://peo.0kj1m.cn

Ruby: s.lines
来源：http://wes.fzhhl.top

C#:   s.Split('\n')
来源：http://wwa.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://ibu.zdbjq.cn

Py:   if not s:
来源：http://yfl.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pfm.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cxc.aizwys.cn

TS:   if (s === "") {}
来源：http://jhs.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://ons.cheryme.top

Go:   if s == "" {}
来源：http://jwo.yj20258.top

Ruby: if s.empty?
来源：http://lyr.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eed.sysykeji.top

[E21] 超长截断加省略号
来源：http://hap.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mud.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jip.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyj.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://shi.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://apd.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://fbc.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mvs.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pkr.gzhubu.top

[E22] 字节长度与字符长度
来源：http://ikb.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rcn.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://usg.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmf.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wsj.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mja.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fgw.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://yyj.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zzl.zdqjudy.top

================================================================================
来源：http://lzh.xinyue.icu

F. 文件与目录
来源：http://gik.tarul.cn

================================================================================
来源：http://hee.feifeiyinyue.top

[F01] 读取整个文件
来源：http://tli.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rie.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://zfa.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://voq.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wai.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fxg.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pnl.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://vyg.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://ghh.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://vth.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ezi.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lzz.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxm.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://urm.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://led.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://exr.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gvc.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kvi.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://rlm.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uwj.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://quy.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrf.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ure.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sjt.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bjc.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://eyb.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ibx.guannengcc.top

[F04] 追加写入文件
来源：http://qzh.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qxt.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wfk.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://top.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xft.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldt.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mko.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fll.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eri.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://eci.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://upl.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://irp.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://aes.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://dzl.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vux.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ixr.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://zfc.yj202588.top

C#:   File.Exists("a.txt")
来源：http://ugj.jqgufenzy.top

[F06] 删除文件
来源：http://atg.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://tzb.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://rcy.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jtx.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://dfi.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://piu.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://ziy.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://kxc.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://znz.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://ryf.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdr.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mzg.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgf.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gmm.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mnx.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mkt.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hvx.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://anf.yueranfly.top

[F08] 遍历目录
来源：http://mzd.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://huo.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hrh.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://nnj.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://zig.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wgz.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://udc.ydzc1.top

Ruby: Dir.children("dir")
来源：http://zhl.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://nlw.daxiang520.top

[F09] 获取文件大小
来源：http://txr.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://usc.yj20258.top

PHP:  filesize("a.txt");
来源：http://hej.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://fgn.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://dtb.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://fyd.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xjg.ydzc1.top

Ruby: File.size("a.txt")
来源：http://mlq.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://yfm.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://edg.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://djj.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lml.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ivd.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://loc.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qny.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qiq.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dqo.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zpu.xuanzx.com

[F11] 复制与移动文件
来源：http://lsx.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jeb.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cxp.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bgu.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mbf.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://djy.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lyd.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fvq.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqs.xziqi.cn

[F12] CSV 读写
来源：http://bit.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pxu.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://agh.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ohw.nwbrower.top

TS:   // 同上
来源：http://mrj.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kbz.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sar.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rhh.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pfl.0kj1m.cn

================================================================================
来源：http://aqk.hysaishi.cn

G. 面向对象
来源：http://gja.cashguo.top

================================================================================
来源：http://jyl.shanyushiyangtech.top

[G01] 定义类
来源：http://vyn.sjlbkw.cn

Py:   class User: pass
来源：http://zke.316326.xyz

PHP:  class User {}
来源：http://cbl.316326.xyz

JS:   class User {}
来源：http://pel.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://viu.nanxuanxn.top

Java: class User {}
来源：http://sil.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://pmo.quarkkingdee.top

Ruby: class User; end
来源：http://awz.aibaodan.cn

C#:   class User {}
来源：http://rpl.gogol.net.cn

[G02] 构造函数
来源：http://isp.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://flz.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://vay.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://dev.sweek.top

TS:   constructor(public name: string) {}
来源：http://qwr.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://ycw.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bmy.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://hgj.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://yzi.tanke756.top

[G03] 实例属性
来源：http://wbk.ybcxt.top

Py:   self.name = "x"
来源：http://tlu.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://gta.jlsjyb.cn

JS:   this.name = "x";
来源：http://aap.gogol.net.cn

TS:   name: string = "x";
来源：http://sbt.snrcjt.cn

Java: private String name;
来源：http://jcc.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cpp.zhijiandao.cn

Ruby: @name = "x"
来源：http://zwg.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://ldm.cashguo.top

[G04] 定义方法
来源：http://pss.sxryk.cn

Py:   def greet(self): return self.name
来源：http://xlb.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ngv.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://ywv.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://riq.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://svc.zhijiandao.cn


<!-- 参考信息 -->