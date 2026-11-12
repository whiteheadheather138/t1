代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://oca.cqqwz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rog.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://upg.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vng.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://drn.havefunace.top

[E07] 按分隔符拆分
来源：http://msn.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dlv.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fll.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yhe.tarul.cn

TS:   s.split(",")
来源：http://gez.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ptc.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ncb.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://rdk.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vdg.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://ymi.jqgufenzy.top

Py:   ",".join(items)
来源：http://trr.nwbrower.top

PHP:  implode(",", $items);
来源：http://bzy.cdnleiting.top

JS:   items.join(",")
来源：http://zhn.yvedp.cn

TS:   items.join(",")
来源：http://ejb.snrcjt.cn

Java: String.join(",", items)
来源：http://xfq.tanke756.top

Go:   strings.Join(items, ",")
来源：http://ajy.yuxming.cn

Ruby: items.join(",")
来源：http://ijx.316326.xyz

C#:   string.Join(",", items)
来源：http://eqq.zdbjq.cn

[E09] 去除所有空白字符
来源：http://vei.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://awh.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://opw.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://kbo.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://xui.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://nli.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fnm.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://eax.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tgu.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://eik.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hye.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://noe.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://cxc.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://vxw.ybcxt.top

Java: String.format("%03d", 7)
来源：http://mos.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cda.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zcl.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywp.fzhhl.top

[E11] 反转字符串
来源：http://rjf.yj20258888.top

Py:   s[::-1]
来源：http://qsg.svipenyu.cn

PHP:  strrev($s);
来源：http://cpc.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://glu.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://dhq.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xie.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://afk.quarkkingdee.top

Ruby: s.reverse
来源：http://yxc.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://lzk.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://xwy.mhx1999.top

Py:   s.count("a")
来源：http://fpq.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://iwy.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://tzi.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://pvl.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vag.316326.xyz

Go:   strings.Count(s, "a")
来源：http://geo.iojbl.cn

Ruby: s.count("a")
来源：http://vnj.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://kep.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://iah.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://ycd.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://udt.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cpb.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qoj.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dox.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gvt.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zuv.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://djl.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://vha.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cjs.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vmo.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tah.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rfr.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qyv.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baz.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uqv.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ccv.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://gol.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kml.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sfe.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pkg.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rpp.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uxv.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mtk.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://byu.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://obn.aibaodan.cn

[E16] 数字千分位
来源：http://lkn.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://qtb.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://qnt.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://ssk.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://miy.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ksg.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lyt.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mli.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://mvk.hnqzz.top

[E17] 首字母大写
来源：http://vcn.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gwg.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://btx.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wql.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yqy.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://keu.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rhh.wangshuangyany.cn

Ruby: s.capitalize
来源：http://lnp.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rlh.zycfv.cn

[E18] 模板占位符替换
来源：http://fwv.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scs.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tor.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://one.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hth.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bax.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pxt.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nid.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nux.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://kgm.uphjek.com

Py:   s.splitlines()
来源：http://qyb.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nqu.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://qcz.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://pza.jianghu66.top

Java: s.lines().toList()
来源：http://lbn.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://nvr.tarul.cn

Ruby: s.lines
来源：http://jpa.316326.xyz

C#:   s.Split('\n')
来源：http://yip.ydzc1.top

[E20] 判断字符串是否为空
来源：http://nij.gogol.net.cn

Py:   if not s:
来源：http://qsc.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tke.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iub.wangdashe.top

TS:   if (s === "") {}
来源：http://kqe.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://trr.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://wkf.jqgufenzy.top

Ruby: if s.empty?
来源：http://hjt.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qdv.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://hkj.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ooa.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://euk.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mnr.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qny.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emx.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://ldz.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wnb.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://svt.52xcode.cn

[E22] 字节长度与字符长度
来源：http://utk.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vod.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sir.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qei.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wuc.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ilo.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dgv.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://zwt.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mvf.ydjk.org.cn

================================================================================
来源：http://gcu.havefunace.top

F. 文件与目录
来源：http://uob.zhoulong.xyz

================================================================================
来源：http://uwy.tian-w.cn

[F01] 读取整个文件
来源：http://kxn.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rmd.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://arw.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lmo.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vqt.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://why.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qop.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://wti.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xll.yj20258.top

[F02] 逐行读取文件
来源：http://wxo.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rfn.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://syo.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tah.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oei.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sla.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pst.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yij.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mrv.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://ezb.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://anc.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oqe.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wkv.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imq.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msh.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lig.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://wil.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://leg.yj20258.top

[F04] 追加写入文件
来源：http://bih.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hfz.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nwv.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwu.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wok.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dpa.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kul.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://urz.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jho.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://deg.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sbm.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://okq.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://fki.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://cxh.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zkb.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ceh.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://shh.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://hql.jinqigufen.top

[F06] 删除文件
来源：http://pcj.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://qrk.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://atg.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rpt.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zae.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sbf.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://tzb.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://tut.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://xfn.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://xme.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pdw.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fnm.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btb.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fzf.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kqd.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hhd.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yoy.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pkm.chenjidiqi.icu

[F08] 遍历目录
来源：http://jbu.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uay.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qab.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://eik.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://hih.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zdx.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tpu.52xcode.cn

Ruby: Dir.children("dir")
来源：http://ocl.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://tmg.ybcxt.top

[F09] 获取文件大小
来源：http://dwa.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ghf.fengsongda.top

PHP:  filesize("a.txt");
来源：http://uhq.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://zrj.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://dou.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tdh.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lza.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://fxj.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://btf.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://amd.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hak.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zeo.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uit.yuxming.cn

TS:   path.extname("a.txt")
来源：http://oid.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ick.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gvb.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iut.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ykw.vqdsnc.cn

[F11] 复制与移动文件
来源：http://uqw.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://okk.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qiw.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwz.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syc.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://izg.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tra.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ubm.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uhx.meibo888.top

[F12] CSV 读写
来源：http://oei.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kik.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uzk.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qua.sxryk.cn

TS:   // 同上
来源：http://tmr.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://isq.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lrs.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wyr.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rzr.havefunace.top

================================================================================
来源：http://rho.xinyue.icu

G. 面向对象
来源：http://mgw.chenzaomai.com

================================================================================
来源：http://uzi.jqgufenzy.top

[G01] 定义类
来源：http://ese.meibo888.top

Py:   class User: pass
来源：http://frx.sjlbkw.cn

PHP:  class User {}
来源：http://nkt.zhoulong.xyz

JS:   class User {}
来源：http://ndv.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://ing.feifeiyinyue.top

Java: class User {}
来源：http://gts.cashguo.top

Go:   type User struct { Name string }
来源：http://hwv.9152youxi.cn

Ruby: class User; end
来源：http://qig.wangshuangyany.cn

C#:   class User {}
来源：http://wxa.9152youxi.cn

[G02] 构造函数
来源：http://oza.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://sut.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://cbf.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://doc.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://jha.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://iju.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dou.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://lob.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://ndy.jinqigufen.top

[G03] 实例属性
来源：http://uqj.smart0.xyz

Py:   self.name = "x"
来源：http://ggm.yuanzhike.top

PHP:  public string $name = "x";
来源：http://znt.nwbrower.top

JS:   this.name = "x";
来源：http://jez.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://cxi.meibo888.top

Java: private String name;
来源：http://xoy.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wqo.xuetiantiany.cn

Ruby: @name = "x"
来源：http://llw.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://yxc.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://kdj.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://ulz.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ztj.nwbrower.top

JS:   greet() { return this.name; }
来源：http://kiz.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://psh.jlsjyb.cn

Java: String greet() { return name; }
来源：http://wyd.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rtd.hnqzz.top

Ruby: def greet; @name; end
来源：http://rym.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://fab.52xcode.cn

[G05] 继承
来源：http://wyn.chenzaomai.com


<!-- 参考信息 -->