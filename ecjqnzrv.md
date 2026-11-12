代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mho.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://erc.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pmv.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iub.yongpay.top

C#:   s.Replace("a", "b")
来源：http://fvt.sufxvd.cn

[E07] 按分隔符拆分
来源：http://gbs.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ppi.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kkd.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ckb.fanxiaobao.xyz

TS:   s.split(",")
来源：http://seq.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://kyh.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yjf.pycfn.com

Ruby: s.split(",");  s.split
来源：http://pvm.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcd.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://umx.cqqwz.cn

Py:   ",".join(items)
来源：http://dsm.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://uov.hongshengwenyu.top

JS:   items.join(",")
来源：http://wbh.ydzc1.top

TS:   items.join(",")
来源：http://dyq.9152youxi.cn

Java: String.join(",", items)
来源：http://zcg.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://tlo.gogol.net.cn

Ruby: items.join(",")
来源：http://krr.xylfe.cn

C#:   string.Join(",", items)
来源：http://aqu.yuanzhike.top

[E09] 去除所有空白字符
来源：http://tqd.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://toi.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mdr.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://ito.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://hkc.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://qtm.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ouk.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://mmx.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rdk.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://pyv.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ufb.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nxl.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://gmi.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://jkb.cashguo.top

Java: String.format("%03d", 7)
来源：http://lza.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://czq.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aup.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ydp.bbcook.cn

[E11] 反转字符串
来源：http://nck.0kj1m.cn

Py:   s[::-1]
来源：http://mwe.0kj1m.cn

PHP:  strrev($s);
来源：http://klm.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://yfh.xuanzx.com

TS:   [...s].reverse().join("")
来源：http://riu.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dpc.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fbs.wangdashe.top

Ruby: s.reverse
来源：http://utf.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://jmh.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://xfc.yanxiufei.cn

Py:   s.count("a")
来源：http://zqy.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://mmx.vehdjk.com

JS:   s.split("a").length - 1
来源：http://ula.andypj.xyz

TS:   s.split("a").length - 1
来源：http://oyw.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fko.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://xrl.9152youxi.cn

Ruby: s.count("a")
来源：http://ext.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://wsp.uphjek.com

[E13] 逐字符遍历
来源：http://fjv.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://yta.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nsa.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yrt.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://anv.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gpv.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dog.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ctk.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lyu.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://bmn.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://moi.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ogt.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vjj.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nyq.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ngw.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ulk.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ewd.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iki.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://wio.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vih.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gjd.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zww.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://lxl.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vus.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hxr.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fvp.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prl.hnxiangtu.top

[E16] 数字千分位
来源：http://soj.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://nkw.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://gme.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://esg.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qmo.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uuk.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fnv.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qib.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://sgo.ppjwa.cn

[E17] 首字母大写
来源：http://imq.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://glj.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vyb.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fod.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dch.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpd.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qsn.zhongyouzk.top

Ruby: s.capitalize
来源：http://lab.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://duu.yj202588.top

[E18] 模板占位符替换
来源：http://eec.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jwz.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lnp.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rzi.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dux.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lte.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kuh.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://riu.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ewc.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://nun.yuxming.cn

Py:   s.splitlines()
来源：http://tia.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oke.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://ozz.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://gju.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://ggn.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://yao.meibo888.top

Ruby: s.lines
来源：http://oaf.c1oappe.top

C#:   s.Split('\n')
来源：http://dbo.aizwys.cn

[E20] 判断字符串是否为空
来源：http://rad.fktsv.cn

Py:   if not s:
来源：http://gqc.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yxn.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wdo.redwolf501.top

TS:   if (s === "") {}
来源：http://gla.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://qgx.0kj1m.cn

Go:   if s == "" {}
来源：http://hke.nwbrower.top

Ruby: if s.empty?
来源：http://fvv.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ucy.jianghu66.top

[E21] 超长截断加省略号
来源：http://zon.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bem.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lmd.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fiz.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xmw.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zmh.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://pxu.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oqi.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xmx.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://pjd.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rdy.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://odq.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxm.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://htb.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bav.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aba.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://dhd.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rvz.ivvv.top

================================================================================
来源：http://wml.yueranfly.top

F. 文件与目录
来源：http://uvy.fengsongda.top

================================================================================
来源：http://ykn.xinyue.icu

[F01] 读取整个文件
来源：http://ofi.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fwt.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://njx.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pxv.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ymk.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fur.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfu.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://uoi.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://mhx.hnxiangtu.top

[F02] 逐行读取文件
来源：http://sga.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wkv.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pzt.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmn.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhm.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jmj.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xlh.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cdp.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rdl.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://ovb.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wlx.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://koj.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ooh.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezv.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dum.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xoz.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://qso.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hjj.nanxuanxn.top

[F04] 追加写入文件
来源：http://oci.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ore.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://niz.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvz.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmj.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ggn.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ddc.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zwj.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jmw.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://xsv.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fbs.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://dxg.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://zhk.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://qlj.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hrm.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vbw.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://wua.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://klb.haohaochexian.top

[F06] 删除文件
来源：http://mry.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://hxk.iojbl.cn

PHP:  unlink("a.txt");
来源：http://nct.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uid.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fws.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldt.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://ofy.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://rhm.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://mby.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://agx.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dkl.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uoa.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvi.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xaq.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kbd.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wzo.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vuw.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dry.havefunace.top

[F08] 遍历目录
来源：http://ggw.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ocf.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufa.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://cna.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://hcs.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nym.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://nwf.bbcook.cn

Ruby: Dir.children("dir")
来源：http://aal.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://jsd.yongpay.top

[F09] 获取文件大小
来源：http://tim.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://rij.fzhhl.top

PHP:  filesize("a.txt");
来源：http://gny.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://ayw.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://bep.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://bds.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ahp.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://vbz.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://dzc.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://ydo.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://epu.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ved.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gzu.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://qji.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gwy.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://krw.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vou.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fop.nwbrower.top

[F11] 复制与移动文件
来源：http://ase.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yci.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zfn.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rbf.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kme.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uuv.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rab.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://brp.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbz.sxryk.cn

[F12] CSV 读写
来源：http://gvr.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnd.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lqm.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fmd.snrcjt.cn

TS:   // 同上
来源：http://qzz.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uax.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://onm.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cvz.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kix.pycfn.com

================================================================================
来源：http://xtd.ybcxt.top

G. 面向对象
来源：http://woq.nwbrower.top

================================================================================
来源：http://sxt.cucudq.cn

[G01] 定义类
来源：http://apv.hywenlv.cn

Py:   class User: pass
来源：http://cbf.feifeiyinyue.top

PHP:  class User {}
来源：http://iqo.cashguo.top

JS:   class User {}
来源：http://rdq.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://lpp.guannengcc.top

Java: class User {}
来源：http://orb.ppjwa.cn

Go:   type User struct { Name string }
来源：http://gwy.aibaodan.cn

Ruby: class User; end
来源：http://uqp.yonumen.top

C#:   class User {}
来源：http://bet.nanxuanxn.top

[G02] 构造函数
来源：http://del.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://uuk.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://lbz.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://kil.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://doo.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://hjr.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://upf.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://ctg.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://inh.yonumen.top

[G03] 实例属性
来源：http://inb.daria6918.cn

Py:   self.name = "x"
来源：http://iop.sufxvd.cn

PHP:  public string $name = "x";
来源：http://wma.zhongyouzk.top

JS:   this.name = "x";
来源：http://gyh.ivvv.top

TS:   name: string = "x";
来源：http://byp.jqgfzy.top

Java: private String name;
来源：http://vbe.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wwq.meibo888.top

Ruby: @name = "x"
来源：http://cxw.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://gco.zdbjq.cn

[G04] 定义方法
来源：http://xcj.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://vzf.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kzm.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://ecz.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://ies.aibaodan.cn

Java: String greet() { return name; }
来源：http://ypz.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xpe.tianlin.xyz

Ruby: def greet; @name; end
来源：http://koa.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://acy.cheryme.top

[G05] 继承
来源：http://fgf.hfpthk.cn


<!-- 参考信息 -->