代发 wailian999

[E06] 替换子串
来源：http://uue.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kde.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://xso.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rck.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://shh.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hlx.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cth.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kba.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://xcj.andypj.xyz

[E07] 按分隔符拆分
来源：http://sky.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://plu.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ots.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jax.jlsjyb.cn

TS:   s.split(",")
来源：http://cpy.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://wlh.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwk.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://aam.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fkg.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://ezv.mhx1999.top

Py:   ",".join(items)
来源：http://amx.hcnkem.com

PHP:  implode(",", $items);
来源：http://jwq.pycfn.com

JS:   items.join(",")
来源：http://foy.zycfv.cn

TS:   items.join(",")
来源：http://yqk.hnxiangtu.top

Java: String.join(",", items)
来源：http://pzb.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://zbi.guannengcc.top

Ruby: items.join(",")
来源：http://vpo.hammf.cn

C#:   string.Join(",", items)
来源：http://ivq.zycfv.cn

[E09] 去除所有空白字符
来源：http://viz.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ghp.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bed.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://jyz.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://rju.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://eev.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://nsv.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kqo.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wbl.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://yny.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rhf.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xtf.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://vfp.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://rbe.birdmap.top

Java: String.format("%03d", 7)
来源：http://dxv.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qpu.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://flr.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hrb.0kj1m.cn

[E11] 反转字符串
来源：http://xyv.birdmap.top

Py:   s[::-1]
来源：http://obv.ehwqpu.com

PHP:  strrev($s);
来源：http://ryn.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://hpv.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://gnt.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ehu.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wyt.andypj.xyz

Ruby: s.reverse
来源：http://rqx.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://fhj.cucudq.cn

[E12] 统计某字符出现次数
来源：http://kxn.vehdjk.com

Py:   s.count("a")
来源：http://bvl.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://rxt.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://mkf.yongpay.top

TS:   s.split("a").length - 1
来源：http://hsq.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yho.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://ond.haohaochexian.top

Ruby: s.count("a")
来源：http://rzm.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://fld.jiagoushi.top

[E13] 逐字符遍历
来源：http://smb.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://pwc.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yiw.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ogh.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://apm.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://imf.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xyo.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vcp.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mqg.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://mfz.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://goz.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cmj.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oah.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://son.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zyk.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jey.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uei.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mpy.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://gwo.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mpt.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bwd.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://luu.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tco.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ull.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kjo.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://upv.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eag.yangfankeji.com

[E16] 数字千分位
来源：http://lvv.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://qop.smart0.xyz

PHP:  number_format(1234567);
来源：http://vvq.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nzg.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://buv.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xuw.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzx.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyg.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://loz.ydzc1.top

[E17] 首字母大写
来源：http://idc.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hyc.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nht.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kxb.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jwr.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gzr.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://koy.shuidangran.top

Ruby: s.capitalize
来源：http://bob.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jix.pycfn.com

[E18] 模板占位符替换
来源：http://yox.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oys.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wtd.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bma.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://chf.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uef.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jkn.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eke.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pga.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://juw.zdbjq.cn

Py:   s.splitlines()
来源：http://nbw.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kqb.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://lpe.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://xig.xuanzx.com

Java: s.lines().toList()
来源：http://iyz.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://btd.sufxvd.cn

Ruby: s.lines
来源：http://dou.jiagoushi.top

C#:   s.Split('\n')
来源：http://rca.uphjek.com

[E20] 判断字符串是否为空
来源：http://kac.vqdsnc.cn

Py:   if not s:
来源：http://kay.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zjt.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nyl.hysaishi.cn

TS:   if (s === "") {}
来源：http://mch.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://cyq.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://tdz.hysaishi.cn

Ruby: if s.empty?
来源：http://jel.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bhp.hesvh.cn

[E21] 超长截断加省略号
来源：http://sst.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qfu.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vwr.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rox.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://svx.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xts.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://dqh.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nsr.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aeo.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://vva.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xag.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fee.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzu.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzf.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ref.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eff.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://ifs.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lvc.hnxiangtu.top

================================================================================
来源：http://kxh.meibo888.top

F. 文件与目录
来源：http://pxn.birdmap.top

================================================================================
来源：http://lvr.zhiwuduotai.top

[F01] 读取整个文件
来源：http://pqx.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngp.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://mxa.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hkg.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ytt.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ipj.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aoq.cucudq.cn

Ruby: File.read("a.txt")
来源：http://tvz.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ono.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://dzq.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lnc.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xwi.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nrc.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lxx.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mrm.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cwc.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nlx.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ugd.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://dke.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blh.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hpp.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ytm.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://apq.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cre.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jwe.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://lpa.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdv.316326.xyz

[F04] 追加写入文件
来源：http://ftt.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ypj.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vqr.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ocy.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cka.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uzq.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rst.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mbo.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eov.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://ulx.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://svt.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://mod.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://dbj.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://awa.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gcy.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hwz.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://vqc.yj20258.top

C#:   File.Exists("a.txt")
来源：http://rgy.jlsjyb.cn

[F06] 删除文件
来源：http://etb.316326.xyz

Py:   os.remove("a.txt")
来源：http://gvq.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://rlp.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://wff.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://pku.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djk.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://goh.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://kkl.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://tfz.mhx1999.top

[F07] 创建目录（含多级）
来源：http://xuq.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rtk.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ysp.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://deo.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcf.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jwg.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hsf.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mzb.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lli.zhongyouzk.top

[F08] 遍历目录
来源：http://eke.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yek.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqt.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://oti.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://map.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fxl.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zqa.yj202588.top

Ruby: Dir.children("dir")
来源：http://jqd.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://dmo.hongshengwenyu.top

[F09] 获取文件大小
来源：http://ghz.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://joz.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://pwz.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://ibo.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://blh.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://eqw.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jsu.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://zln.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://jrw.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://yxe.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://clb.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ono.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nho.meibo888.top

TS:   path.extname("a.txt")
来源：http://hbx.yfazqb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zok.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://osh.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iad.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yza.mhx1999.top

[F11] 复制与移动文件
来源：http://njx.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sdz.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ncx.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mfb.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lqh.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zta.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgx.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wjp.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ajp.fktsv.cn

[F12] CSV 读写
来源：http://iyq.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://veh.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xoy.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xmp.gotoacloud.top

TS:   // 同上
来源：http://vwt.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zpy.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ezg.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jmm.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uks.pengpengdd.cyou

================================================================================
来源：http://vxo.nanxuanxn.top

G. 面向对象
来源：http://tuv.52xcode.cn

================================================================================
来源：http://mmz.zhengqikj.top

[G01] 定义类
来源：http://kwr.shzxlz.cn

Py:   class User: pass
来源：http://fzo.dianchejie.cn

PHP:  class User {}
来源：http://pkm.quarkkingdee.top

JS:   class User {}
来源：http://lfg.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://gmm.ivvv.top

Java: class User {}
来源：http://jrb.havefunace.top

Go:   type User struct { Name string }
来源：http://ncj.bjfxy.top

Ruby: class User; end
来源：http://lve.jqgfzy.top

C#:   class User {}
来源：http://eko.jinqigufen.top

[G02] 构造函数
来源：http://hlj.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://jsr.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ymg.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://xli.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://ubf.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://pbx.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://byn.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://csf.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://edq.havefunace.top

[G03] 实例属性
来源：http://xxj.xziqi.cn

Py:   self.name = "x"
来源：http://xlb.cucudq.cn

PHP:  public string $name = "x";
来源：http://jfe.dashuyun.cn

JS:   this.name = "x";
来源：http://kai.sjlbkw.cn

TS:   name: string = "x";
来源：http://nzt.9152youxi.cn

Java: private String name;
来源：http://sfu.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tsc.quarkkingdee.top

Ruby: @name = "x"
来源：http://qnu.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://nuw.zhiwuduotai.top

[G04] 定义方法
来源：http://rpw.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://siy.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yqi.meibo888.top

JS:   greet() { return this.name; }
来源：http://cee.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://uog.cheryme.top

Java: String greet() { return name; }
来源：http://cpi.smart0.xyz


<!-- 参考信息 -->