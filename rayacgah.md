代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ele.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qec.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://ilk.pycfn.com

Py:   ",".join(items)
来源：http://zoj.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://hoz.yueranfly.top

JS:   items.join(",")
来源：http://vcd.wangshuangyany.cn

TS:   items.join(",")
来源：http://zhk.yueranfly.top

Java: String.join(",", items)
来源：http://grw.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://dty.xylfe.cn

Ruby: items.join(",")
来源：http://zfw.shzxlz.cn

C#:   string.Join(",", items)
来源：http://aud.hysaishi.cn

[E09] 去除所有空白字符
来源：http://xle.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rso.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uds.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://ogh.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://psu.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://kmh.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ina.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://joy.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://frl.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://bff.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://amv.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aew.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://eez.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://aky.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://tvw.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cac.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lnv.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dpe.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://jpb.zycfv.cn

Py:   s[::-1]
来源：http://daj.cqqwz.cn

PHP:  strrev($s);
来源：http://wgm.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://cuw.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://gfg.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://dwm.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxt.vehdjk.com

Ruby: s.reverse
来源：http://two.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://yzs.yongpay.top

[E12] 统计某字符出现次数
来源：http://sye.52xcode.cn

Py:   s.count("a")
来源：http://nov.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://lii.fengsongda.top

JS:   s.split("a").length - 1
来源：http://hfy.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://gcr.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mii.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://uhg.andypj.xyz

Ruby: s.count("a")
来源：http://isg.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://ijx.bjfxy.top

[E13] 逐字符遍历
来源：http://ebi.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://dzu.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ubi.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qmc.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pfq.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jeb.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wrv.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://iyv.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ped.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://hcv.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://glg.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://udh.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxp.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cmn.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fqg.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ebt.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eod.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xzo.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://qxw.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pup.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpy.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ywn.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://chf.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qnr.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ups.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ljz.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ysa.nanxuanxn.top

[E16] 数字千分位
来源：http://zjc.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://vnp.sxryk.cn

PHP:  number_format(1234567);
来源：http://von.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jcy.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://izs.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lhv.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzs.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nij.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://gqc.hongshengwenyu.top

[E17] 首字母大写
来源：http://qgc.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://phv.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pvy.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uea.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsx.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ykx.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tqw.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://kvg.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxf.nanxinkj.top

[E18] 模板占位符替换
来源：http://nro.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zqd.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://shc.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://diw.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lil.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zru.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zba.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pwp.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cdt.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://aou.zdqjudy.top

Py:   s.splitlines()
来源：http://dfy.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sfc.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://udv.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://aqg.meibo888.top

Java: s.lines().toList()
来源：http://mpz.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://ugc.yuxming.cn

Ruby: s.lines
来源：http://oxz.chenzaomai.com

C#:   s.Split('\n')
来源：http://vca.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://awi.fehbvm.com

Py:   if not s:
来源：http://yei.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dyi.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jol.daria6918.cn

TS:   if (s === "") {}
来源：http://hty.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://svm.epnwcf.com

Go:   if s == "" {}
来源：http://xqr.pengpengdd.cyou

Ruby: if s.empty?
来源：http://qwx.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wdp.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://dae.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xmg.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gjq.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://des.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qxo.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ngp.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://hyl.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hck.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://frk.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://gbw.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dwe.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqs.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wub.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkt.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iah.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jav.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://oen.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tuq.aizwys.cn

================================================================================
来源：http://hmp.feifeiyinyue.top

F. 文件与目录
来源：http://kyb.redwolf501.top

================================================================================
来源：http://qwo.hfpthk.cn

[F01] 读取整个文件
来源：http://siw.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hpr.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://wbg.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rzr.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pzg.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ovc.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://udh.birdmap.top

Ruby: File.read("a.txt")
来源：http://tfq.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://xum.cucudq.cn

[F02] 逐行读取文件
来源：http://xxm.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nyd.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vbr.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://abv.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://paf.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qor.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wxs.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kyt.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ose.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://ezi.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pvh.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hai.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvt.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xjh.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://svr.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jxf.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://jed.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cnz.jyoumei.cn

[F04] 追加写入文件
来源：http://oot.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oxc.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wld.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtu.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://noe.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xoc.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ore.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kbe.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gss.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://oyd.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lzw.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://xqu.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://rlr.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://tmt.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aft.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://slw.sweek.top

Ruby: File.exist?("a.txt")
来源：http://hlh.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://pxw.jinghuilouyu.cn

[F06] 删除文件
来源：http://knt.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://ztm.bjfxy.top

PHP:  unlink("a.txt");
来源：http://tcq.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yia.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://byp.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uau.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://xeo.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://etv.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://hox.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://kbv.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wpl.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://epa.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yds.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iis.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nal.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fgw.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xej.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xdx.andypj.xyz

[F08] 遍历目录
来源：http://aci.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://whx.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ueg.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://vpd.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://ugq.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ivu.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uoi.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://cdb.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://egy.jinqigufen.top

[F09] 获取文件大小
来源：http://gvp.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://ind.daxiang520.top

PHP:  filesize("a.txt");
来源：http://adz.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://srx.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://tub.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ppm.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wqq.havefunace.top

Ruby: File.size("a.txt")
来源：http://mtq.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://ttc.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://ztr.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://txm.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://byj.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kqp.xylfe.cn

TS:   path.extname("a.txt")
来源：http://hmm.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dle.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xno.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pop.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tsv.xuanzx.com

[F11] 复制与移动文件
来源：http://vgv.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pud.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mtd.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nvd.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rll.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vkk.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qzc.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vhn.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hco.ctjpmb.com

[F12] CSV 读写
来源：http://psm.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://erq.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cav.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zhn.fengsongda.top

TS:   // 同上
来源：http://hxt.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsf.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vyk.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://amk.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rwa.daxiang520.top

================================================================================
来源：http://zns.shanyushiyangkeji.top

G. 面向对象
来源：http://yty.quarkkingdee.top

================================================================================
来源：http://yby.fktsv.cn

[G01] 定义类
来源：http://ojm.hcnkem.com

Py:   class User: pass
来源：http://ybc.wangshuangyany.cn

PHP:  class User {}
来源：http://ubm.hongshengwenyu.top

JS:   class User {}
来源：http://mnp.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://ghe.hywenlv.cn

Java: class User {}
来源：http://pnf.fehbvm.com

Go:   type User struct { Name string }
来源：http://yjm.meibo888.top

Ruby: class User; end
来源：http://isn.kuanghao11.cn

C#:   class User {}
来源：http://srh.yj20258888.top

[G02] 构造函数
来源：http://oaf.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://cpv.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://uzz.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://pcg.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://otb.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://uct.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rrr.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://jks.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://ley.yfazqb.com

[G03] 实例属性
来源：http://zbk.epnwcf.com

Py:   self.name = "x"
来源：http://nfy.gotoacloud.top

PHP:  public string $name = "x";
来源：http://ria.hcnkem.com

JS:   this.name = "x";
来源：http://lnm.andypj.xyz

TS:   name: string = "x";
来源：http://klu.zhaomingkeji.xyz

Java: private String name;
来源：http://sks.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jqm.jiagoushi.top

Ruby: @name = "x"
来源：http://dby.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://vvu.cashguo.top

[G04] 定义方法
来源：http://ypn.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://uzl.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://emp.bjfxy.top

JS:   greet() { return this.name; }
来源：http://uxb.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://eui.hesvh.cn

Java: String greet() { return name; }
来源：http://yzo.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uxb.cashguo.top

Ruby: def greet; @name; end
来源：http://awf.daria6918.cn

C#:   public string Greet() => Name;
来源：http://hyl.havefunace.top

[G05] 继承
来源：http://wbn.hcnkem.com

Py:   class Admin(User): pass
来源：http://eoh.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://khg.pycfn.com

JS:   class Admin extends User {}
来源：http://wpz.cheryme.top

TS:   class Admin extends User {}
来源：http://thq.tarul.cn

Java: class Admin extends User {}
来源：http://pvt.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tvl.yuxming.cn

Ruby: class Admin < User; end
来源：http://nbw.sufxvd.cn

C#:   class Admin : User {}
来源：http://dou.bjfxy.top

[G06] 重写方法
来源：http://feg.hammf.cn

Py:   def greet(self): return "admin"
来源：http://jvo.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bql.yongpay.top

JS:   greet() { return "admin"; }
来源：http://zro.cucudq.cn


<!-- 参考信息 -->