代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://wyl.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kkz.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kyl.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kdm.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://dmq.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://hcj.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ccu.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oaf.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://upw.zdqjudy.top

TS:   s.split(",")
来源：http://xbj.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://exv.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bob.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://nja.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ajz.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://cys.jyoumei.cn

Py:   ",".join(items)
来源：http://cwh.zdqjudy.top

PHP:  implode(",", $items);
来源：http://pep.jinghuilouyu.cn

JS:   items.join(",")
来源：http://xtk.hfpthk.cn

TS:   items.join(",")
来源：http://tfi.chenjidiqi.icu

Java: String.join(",", items)
来源：http://kpe.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://kjt.sysykeji.top

Ruby: items.join(",")
来源：http://wxp.guannengcc.top

C#:   string.Join(",", items)
来源：http://uvk.hywenlv.cn

[E09] 去除所有空白字符
来源：http://zis.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tfn.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://czv.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://ims.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://ldh.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://okh.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eqm.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://ysc.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://loz.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://yna.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://toq.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://puv.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://jby.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://ctl.yonumen.top

Java: String.format("%03d", 7)
来源：http://jat.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pip.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://veu.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ujt.yj202588.top

[E11] 反转字符串
来源：http://gau.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://ckd.dashuyun.cn

PHP:  strrev($s);
来源：http://yio.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://jup.yj20258.top

TS:   [...s].reverse().join("")
来源：http://jtv.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://apo.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xpd.haohaochexian.top

Ruby: s.reverse
来源：http://tji.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jwp.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://kvm.ppjwa.cn

Py:   s.count("a")
来源：http://itw.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://vjb.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://nvx.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://elf.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://non.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://nsn.vqdsnc.cn

Ruby: s.count("a")
来源：http://zgn.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://rzc.daria6918.cn

[E13] 逐字符遍历
来源：http://glq.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://xzt.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dbq.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://odb.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qbk.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vzb.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wza.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pmi.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gax.aizwys.cn

[E14] URL 编码与 Base64
来源：http://ink.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://key.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nqo.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sdm.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xde.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jiw.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bhs.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dad.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iuj.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://pvh.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ewh.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://swk.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yow.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jtr.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kov.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bed.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oyf.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmr.hongshengwenyu.top

[E16] 数字千分位
来源：http://qih.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://wkn.hywenlv.cn

PHP:  number_format(1234567);
来源：http://tqv.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rbw.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xbt.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pgz.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kbm.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zxh.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://ble.xuanzx.com

[E17] 首字母大写
来源：http://eaq.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dfk.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oxk.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pus.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhm.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lqu.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kwz.gzhubu.top

Ruby: s.capitalize
来源：http://udy.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://che.hesvh.cn

[E18] 模板占位符替换
来源：http://rbn.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mcz.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pcz.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://daz.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yer.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cdz.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ifv.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bsx.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ewn.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://eqj.yuanzhike.top

Py:   s.splitlines()
来源：http://eoc.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blj.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://wpg.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://dsc.xinyue.icu

Java: s.lines().toList()
来源：http://jlb.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://cea.yuxming.cn

Ruby: s.lines
来源：http://wsp.jyoumei.cn

C#:   s.Split('\n')
来源：http://bkg.hesvh.cn

[E20] 判断字符串是否为空
来源：http://jtx.bbcook.cn

Py:   if not s:
来源：http://mnu.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhp.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rfi.ydjk.org.cn

TS:   if (s === "") {}
来源：http://yll.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://yjk.jinqigfzy.top

Go:   if s == "" {}
来源：http://ixd.52xcode.cn

Ruby: if s.empty?
来源：http://ydc.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nch.52xcode.cn

[E21] 超长截断加省略号
来源：http://rjr.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qqf.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvf.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lyi.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wgu.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dag.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://miw.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://voh.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fcj.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://efx.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kln.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gik.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ypz.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aso.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mat.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iye.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://bvd.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tps.smart0.xyz

================================================================================
来源：http://zlq.tianlin.xyz

F. 文件与目录
来源：http://sih.bjfxy.top

================================================================================
来源：http://ocu.ydzc1.top

[F01] 读取整个文件
来源：http://ugj.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rob.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://geb.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gts.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tnh.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pxr.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qtj.daria6918.cn

Ruby: File.read("a.txt")
来源：http://jba.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://ryz.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://pzc.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vpb.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mjd.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qkb.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uqx.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fqb.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uxk.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qoe.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jap.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://ogj.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eoq.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ahq.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oke.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mut.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ikb.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsw.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://usq.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zjc.andypj.xyz

[F04] 追加写入文件
来源：http://qqz.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://szb.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qye.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xaa.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtl.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jff.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tez.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nzh.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://slr.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://meg.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vew.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://srf.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://idm.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ysg.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://acm.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wjt.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://eud.tanke756.top

C#:   File.Exists("a.txt")
来源：http://qvj.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://wxu.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://qfz.xylfe.cn

PHP:  unlink("a.txt");
来源：http://lsp.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nkf.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://eit.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uix.uphjek.com

Go:   os.Remove("a.txt")
来源：http://eex.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://urh.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://ugo.gzhubu.top

[F07] 创建目录（含多级）
来源：http://pyk.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehv.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qbr.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmj.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovk.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uol.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cqy.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://osh.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nzz.hywenlv.cn

[F08] 遍历目录
来源：http://klp.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mfb.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://djh.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://fnp.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://azr.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://puj.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://crj.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://ooi.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://ydx.yongpay.top

[F09] 获取文件大小
来源：http://tzj.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://kqn.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://jpc.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://rxh.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://kfc.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://vgx.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mff.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://cee.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://mst.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://ztp.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hgl.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cdj.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://twz.fzhhl.top

TS:   path.extname("a.txt")
来源：http://xsl.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xrx.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wkj.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hsd.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://udk.iojbl.cn

[F11] 复制与移动文件
来源：http://fgw.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bcl.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://crc.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://giv.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfe.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://val.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lxy.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://upz.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jim.jinghuilouyu.cn

[F12] CSV 读写
来源：http://cyy.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wke.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bad.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://doe.ywan-chungtsiang.top

TS:   // 同上
来源：http://hon.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bna.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dfv.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypd.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nvk.meibo888.top

================================================================================
来源：http://gth.hysaishi.cn

G. 面向对象
来源：http://row.0kj1m.cn

================================================================================
来源：http://vdv.jinqigufen.top

[G01] 定义类
来源：http://xnz.nanxinkj.top

Py:   class User: pass
来源：http://vrj.ydjk.org.cn

PHP:  class User {}
来源：http://bjf.dianchejie.cn

JS:   class User {}
来源：http://qmm.ivvv.top

TS:   class User { name: string = ""; }
来源：http://atk.xylfe.cn

Java: class User {}
来源：http://cdz.ivvv.top

Go:   type User struct { Name string }
来源：http://aoh.zdbjq.cn

Ruby: class User; end
来源：http://rjj.hammf.cn

C#:   class User {}
来源：http://qqo.c1oappe.top

[G02] 构造函数
来源：http://xry.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://syl.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://pbv.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://ayi.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://fue.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://flg.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uke.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://ctn.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://eic.dashuyun.cn

[G03] 实例属性
来源：http://omn.nanxuanxn.top

Py:   self.name = "x"
来源：http://xsq.hammf.cn

PHP:  public string $name = "x";
来源：http://oyd.hcnkem.com

JS:   this.name = "x";
来源：http://asi.nwbrower.top

TS:   name: string = "x";
来源：http://lbx.guannengcc.top

Java: private String name;
来源：http://stu.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksf.yj20258888.top

Ruby: @name = "x"
来源：http://hsy.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://dgt.jianghu66.top

[G04] 定义方法
来源：http://maz.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://fky.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nxr.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://myh.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://dhf.tarul.cn

Java: String greet() { return name; }
来源：http://prj.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qrx.mhx1999.top

Ruby: def greet; @name; end
来源：http://afr.andypj.xyz

C#:   public string Greet() => Name;
来源：http://dsr.ydjk.org.cn

[G05] 继承
来源：http://flt.yj202588.top


<!-- 参考信息 -->