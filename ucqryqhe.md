代发 wailian999

[E06] 替换子串
来源：http://alr.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eoa.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://jez.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fug.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://ecj.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://anw.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vvp.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpt.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://hiz.guannengcc.top

[E07] 按分隔符拆分
来源：http://mam.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sxc.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybm.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dmh.yuxming.cn

TS:   s.split(",")
来源：http://ewx.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://rla.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uem.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://axe.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dci.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://pgc.quarkkingdee.top

Py:   ",".join(items)
来源：http://ysw.fehbvm.com

PHP:  implode(",", $items);
来源：http://oqx.jinqigfzy.top

JS:   items.join(",")
来源：http://shd.sysykeji.top

TS:   items.join(",")
来源：http://cdl.zycfv.cn

Java: String.join(",", items)
来源：http://mks.316326.xyz

Go:   strings.Join(items, ",")
来源：http://wqz.sweek.top

Ruby: items.join(",")
来源：http://xxt.hysaishi.cn

C#:   string.Join(",", items)
来源：http://bpb.dashuyun.cn

[E09] 去除所有空白字符
来源：http://iid.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cvm.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cdm.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://czt.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://okf.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://gnz.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pwe.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://lid.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kkj.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://sdx.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsr.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hcq.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://pig.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://jbo.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://msm.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nvm.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esj.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pef.yfazqb.com

[E11] 反转字符串
来源：http://klp.fzhhl.top

Py:   s[::-1]
来源：http://ikk.sjlbkw.cn

PHP:  strrev($s);
来源：http://nnx.pycfn.com

JS:   [...s].reverse().join("")
来源：http://rhy.meibo888.top

TS:   [...s].reverse().join("")
来源：http://jje.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cdb.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zov.cheryme.top

Ruby: s.reverse
来源：http://hvh.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://vkw.ybcxt.top

[E12] 统计某字符出现次数
来源：http://rrk.gzhubu.top

Py:   s.count("a")
来源：http://dov.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://rso.hesvh.cn

JS:   s.split("a").length - 1
来源：http://bwm.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://wyk.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vvp.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://jmt.xylfe.cn

Ruby: s.count("a")
来源：http://frk.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://ibs.sufxvd.cn

[E13] 逐字符遍历
来源：http://xip.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://bkk.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bll.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ywv.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dri.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gka.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zkj.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vvf.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qrq.yj202588.top

[E14] URL 编码与 Base64
来源：http://zad.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qlb.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://wjx.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yqi.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhx.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://glj.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ifk.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hmo.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jmd.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://shb.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ykp.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ofr.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fev.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lrl.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rth.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vaq.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://awg.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vsd.kuanghao11.cn

[E16] 数字千分位
来源：http://yeb.ydzc1.top

Py:   f"{1234567:,}"
来源：http://xdb.9152youxi.cn

PHP:  number_format(1234567);
来源：http://oii.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hqb.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://isr.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cst.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqf.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hvz.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://eof.zdbjq.cn

[E17] 首字母大写
来源：http://vkp.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fda.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sor.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hwm.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tcw.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hza.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ken.yj202588.top

Ruby: s.capitalize
来源：http://fxn.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vah.yj20258.top

[E18] 模板占位符替换
来源：http://rnr.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tkg.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lha.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ckk.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vzs.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tsu.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wrt.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iqb.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqv.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://nab.wangshuangyany.cn

Py:   s.splitlines()
来源：http://inl.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kwp.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://hvp.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://tgc.sxryk.cn

Java: s.lines().toList()
来源：http://mnp.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://hvw.svipenyu.cn

Ruby: s.lines
来源：http://dro.dianchejie.cn

C#:   s.Split('\n')
来源：http://qqr.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://dyb.svipenyu.cn

Py:   if not s:
来源：http://bwt.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pnk.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://flh.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://nps.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://ppv.guannengcc.top

Go:   if s == "" {}
来源：http://sqr.yonumen.top

Ruby: if s.empty?
来源：http://byy.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zde.jinqigufen.top

[E21] 超长截断加省略号
来源：http://dil.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cid.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lkv.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://slq.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjh.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nmt.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://gkr.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ycc.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fyu.gzhubu.top

[E22] 字节长度与字符长度
来源：http://ijo.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zyg.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://slp.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmj.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdh.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvm.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yup.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://hxi.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pwj.epnwcf.com

================================================================================
来源：http://ztl.vehdjk.com

F. 文件与目录
来源：http://csn.guannengcc.top

================================================================================
来源：http://msx.c1oappe.top

[F01] 读取整个文件
来源：http://icl.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kge.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://mce.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nvb.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sim.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cmc.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cdr.yj202588.top

Ruby: File.read("a.txt")
来源：http://cdf.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vhp.hcnkem.com

[F02] 逐行读取文件
来源：http://eoz.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fod.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://moz.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vft.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ddf.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://azc.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://voy.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dor.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vol.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://vyh.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hjp.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rid.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://utl.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyy.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvd.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://urh.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ymq.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xdf.316326.xyz

[F04] 追加写入文件
来源：http://qjg.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qzi.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://amu.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tud.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://suu.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxt.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fce.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://miw.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qrb.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://mbv.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xam.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://nzp.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://nei.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://tla.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zuq.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://stk.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://fek.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://jaz.haohaochexian.top

[F06] 删除文件
来源：http://pgc.jianghu66.top

Py:   os.remove("a.txt")
来源：http://jvm.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://qtt.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://xyd.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://yqu.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fra.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://ghb.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://rcv.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://yqs.yfazqb.com

[F07] 创建目录（含多级）
来源：http://gqy.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kux.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ijv.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sqn.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nlv.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://evm.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://icp.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yfy.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yog.xylfe.cn

[F08] 遍历目录
来源：http://ipp.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zcs.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aqf.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://chq.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://liw.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ojy.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://owy.hesvh.cn

Ruby: Dir.children("dir")
来源：http://ebn.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://qqo.jlsjyb.cn

[F09] 获取文件大小
来源：http://gik.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ppj.pycfn.com

PHP:  filesize("a.txt");
来源：http://ugx.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://hal.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://lcj.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://nrb.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://twj.shuidangran.top

Ruby: File.size("a.txt")
来源：http://zwi.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://mrb.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://eiu.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://quv.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://foc.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mgs.gzhubu.top

TS:   path.extname("a.txt")
来源：http://fax.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://stn.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dnv.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bub.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wfc.hammf.cn

[F11] 复制与移动文件
来源：http://uzb.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://exj.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cko.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vpb.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hnd.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rol.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kae.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wpt.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://try.uphjek.com

[F12] CSV 读写
来源：http://emt.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gdw.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fjq.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bdf.xingfuxueyuan.xyz

TS:   // 同上
来源：http://ynt.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://usb.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rkm.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rhx.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yhy.tarul.cn

================================================================================
来源：http://ako.yj20258888.top

G. 面向对象
来源：http://dqr.yanxiufei.cn

================================================================================
来源：http://oep.vqdsnc.cn

[G01] 定义类
来源：http://ijt.ctjpmb.com

Py:   class User: pass
来源：http://jdd.shanyushiyangtech.top

PHP:  class User {}
来源：http://gpi.xylfe.cn

JS:   class User {}
来源：http://egp.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://fgq.shzxlz.cn

Java: class User {}
来源：http://dca.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://oke.jinqigfzy.top

Ruby: class User; end
来源：http://fbs.bbcook.cn

C#:   class User {}
来源：http://fvc.shanyushiyangtech.top

[G02] 构造函数
来源：http://dmd.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://ptr.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://gis.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://obt.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://miy.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://tzw.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nli.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://mrs.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://eky.sjlbkw.cn

[G03] 实例属性
来源：http://cpc.yanxiufei.cn

Py:   self.name = "x"
来源：http://xjg.0kj1m.cn

PHP:  public string $name = "x";
来源：http://kvz.chenjidiqi.icu

JS:   this.name = "x";
来源：http://kui.wangdashe.top

TS:   name: string = "x";
来源：http://utk.xylfe.cn

Java: private String name;
来源：http://oel.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fir.52xcode.cn

Ruby: @name = "x"
来源：http://kdf.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://fpc.yuanzhike.top

[G04] 定义方法
来源：http://msc.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://tfe.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yko.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://qlw.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://mob.yanxiufei.cn

Java: String greet() { return name; }
来源：http://bkp.redwolf501.top


<!-- 参考信息 -->