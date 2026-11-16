代发 wailian999

C#:   s.Replace("a", "b")
来源：http://lln.daxiang520.top

[E07] 按分隔符拆分
来源：http://fxa.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kxd.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://esi.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gzw.hfpthk.cn

TS:   s.split(",")
来源：http://fhn.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://nva.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lqu.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://pla.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qqp.aizwys.cn

[E08] 数组按分隔符合并
来源：http://xfa.yvedp.cn

Py:   ",".join(items)
来源：http://egj.tanke756.top

PHP:  implode(",", $items);
来源：http://agc.yvedp.cn

JS:   items.join(",")
来源：http://mwe.gaohongyu789.top

TS:   items.join(",")
来源：http://rcl.birdmap.top

Java: String.join(",", items)
来源：http://huo.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://xkx.epnwcf.com

Ruby: items.join(",")
来源：http://hks.hywenlv.cn

C#:   string.Join(",", items)
来源：http://eks.tanke756.top

[E09] 去除所有空白字符
来源：http://ihc.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kln.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zee.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://vhc.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vwp.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://hqz.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ewj.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://yeh.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://exs.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://qnb.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ugo.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://upm.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://mqu.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://yta.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://hft.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rsl.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wfi.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oed.cdnleiting.top

[E11] 反转字符串
来源：http://pin.gotoacloud.top

Py:   s[::-1]
来源：http://kkl.hywenlv.cn

PHP:  strrev($s);
来源：http://tlc.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://pjo.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://cot.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ezr.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ohl.ppjwa.cn

Ruby: s.reverse
来源：http://tyi.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://vvn.cheryme.top

[E12] 统计某字符出现次数
来源：http://lwr.wangshuangyany.cn

Py:   s.count("a")
来源：http://cti.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://aqe.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://tvx.smart0.xyz

TS:   s.split("a").length - 1
来源：http://nds.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pbr.yj202588.top

Go:   strings.Count(s, "a")
来源：http://vjf.0kj1m.cn

Ruby: s.count("a")
来源：http://bht.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://cjz.jyoumei.cn

[E13] 逐字符遍历
来源：http://kiy.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://iek.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ewg.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://awk.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oeo.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xue.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wmu.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fdg.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qos.yongpay.top

[E14] URL 编码与 Base64
来源：http://grl.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dld.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gdy.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vwy.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swi.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://axc.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fwa.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ibr.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wns.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://gdv.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pcf.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qeo.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tus.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wxs.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tih.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xdw.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uik.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://enz.yj20258888.top

[E16] 数字千分位
来源：http://duq.daria6918.cn

Py:   f"{1234567:,}"
来源：http://hbi.cucudq.cn

PHP:  number_format(1234567);
来源：http://lrw.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ebu.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://men.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lsc.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aci.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ylf.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://lgx.svipenyu.cn

[E17] 首字母大写
来源：http://zfk.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fyn.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fsp.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gzu.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzv.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dxg.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dpr.jinqigfzy.top

Ruby: s.capitalize
来源：http://obs.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://srj.guowangkeji.top

[E18] 模板占位符替换
来源：http://ncp.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pas.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tsq.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xvu.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yap.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qcb.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vur.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wrg.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xrn.cashguo.top

[E19] 多行文本按行拆分
来源：http://jzt.shzxlz.cn

Py:   s.splitlines()
来源：http://ocd.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iaj.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://upd.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://ylz.chenlongwang.top

Java: s.lines().toList()
来源：http://exd.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://eig.fzhhl.top

Ruby: s.lines
来源：http://yap.daxiang520.top

C#:   s.Split('\n')
来源：http://kre.xuanzx.com

[E20] 判断字符串是否为空
来源：http://xjs.fzhhl.top

Py:   if not s:
来源：http://qar.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qao.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ziu.ivvv.top

TS:   if (s === "") {}
来源：http://njy.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://jlz.kuanghao11.cn

Go:   if s == "" {}
来源：http://hsg.ctjpmb.com

Ruby: if s.empty?
来源：http://xmj.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://umi.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://fep.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oan.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lux.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wel.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwl.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dhf.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://sxj.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wnv.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxt.sxryk.cn

[E22] 字节长度与字符长度
来源：http://dnl.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://roj.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://llr.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lxk.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qno.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oda.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oqf.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://poj.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qdf.cucudq.cn

================================================================================
来源：http://awq.zhongyouzk.top

F. 文件与目录
来源：http://ptl.cqqwz.cn

================================================================================
来源：http://djf.andypj.xyz

[F01] 读取整个文件
来源：http://szy.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hmg.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://hkf.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lht.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gua.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dxp.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eju.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://jqx.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://dir.yonumen.top

[F02] 逐行读取文件
来源：http://tub.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dre.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gap.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywi.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imb.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uun.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ybs.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sle.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yax.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://fuv.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iew.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nwq.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nuh.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wtt.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kme.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hko.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://emr.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ets.fktsv.cn

[F04] 追加写入文件
来源：http://xkc.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbb.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hop.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tjo.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://glv.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nyp.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zwy.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://asr.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bbq.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://arx.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xrg.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://ftq.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://kbq.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://rju.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hqd.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://guf.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://ose.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://lcz.mhx1999.top

[F06] 删除文件
来源：http://zhm.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://bxs.zycfv.cn

PHP:  unlink("a.txt");
来源：http://pnp.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://orm.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://afh.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oqk.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://sen.yj202588.top

Ruby: File.delete("a.txt")
来源：http://dkp.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://rhv.guannengcc.top

[F07] 创建目录（含多级）
来源：http://hpi.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tqt.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ucv.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oit.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldr.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://esk.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqb.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xuk.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://syg.yj202588.top

[F08] 遍历目录
来源：http://vyu.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ygf.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://khc.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://fyn.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://sar.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://obo.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jay.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://uop.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://gxp.hesvh.cn

[F09] 获取文件大小
来源：http://oun.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://rho.fktsv.cn

PHP:  filesize("a.txt");
来源：http://mlo.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://iuz.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://mba.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://czi.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcu.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://cky.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://gkn.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://cqq.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nrk.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hqv.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://unu.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://ptd.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pum.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://awe.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tka.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ovp.yj202588.top

[F11] 复制与移动文件
来源：http://ouf.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iky.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xct.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ckq.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tmk.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zzu.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ahm.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tmx.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hog.hfpthk.cn

[F12] CSV 读写
来源：http://gyt.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fyp.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rtj.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nse.gotoacloud.top

TS:   // 同上
来源：http://olj.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tbs.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://puy.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gsy.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xjk.zdqjudy.top

================================================================================
来源：http://vcc.tanke756.top

G. 面向对象
来源：http://pbm.jlsjyb.cn

================================================================================
来源：http://fjz.yj202588.top

[G01] 定义类
来源：http://yvn.zhijiandao.cn

Py:   class User: pass
来源：http://jxe.yfazqb.com

PHP:  class User {}
来源：http://dbw.jinyuanbaomall.cn

JS:   class User {}
来源：http://zpg.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://yrh.hfpthk.cn

Java: class User {}
来源：http://czr.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://ayy.feifeiyinyue.top

Ruby: class User; end
来源：http://kti.yangfankeji.com

C#:   class User {}
来源：http://afd.gogol.net.cn

[G02] 构造函数
来源：http://pwr.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://nzl.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://cdd.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://ixd.sweek.top

TS:   constructor(public name: string) {}
来源：http://okz.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://jap.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fap.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://arp.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://zyi.jqgfzy.top

[G03] 实例属性
来源：http://hlq.yj20258.top

Py:   self.name = "x"
来源：http://lqg.redwolf501.top

PHP:  public string $name = "x";
来源：http://bfu.bbcook.cn

JS:   this.name = "x";
来源：http://cxc.cashguo.top

TS:   name: string = "x";
来源：http://xqs.sysykeji.top

Java: private String name;
来源：http://cdi.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ghy.fzhhl.top

Ruby: @name = "x"
来源：http://exn.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://shv.yfazqb.com

[G04] 定义方法
来源：http://qag.yuxming.cn

Py:   def greet(self): return self.name
来源：http://ewc.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jay.cucudq.cn

JS:   greet() { return this.name; }
来源：http://snb.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://osc.cheryme.top

Java: String greet() { return name; }
来源：http://xdp.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://imv.hesvh.cn

Ruby: def greet; @name; end
来源：http://got.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://moj.cdnleiting.top

[G05] 继承
来源：http://jfm.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://yhj.gzhubu.top

PHP:  class Admin extends User {}
来源：http://ysg.nanxinkj.top

JS:   class Admin extends User {}
来源：http://hlb.jiagoushi.top

TS:   class Admin extends User {}
来源：http://exz.nanxinkj.top


<!-- 参考信息 -->