代发 wailian999

C#:   s.Replace("a", "b")
来源：http://kdc.guowangkeji.top

[E07] 按分隔符拆分
来源：http://rpn.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ehf.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nps.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kfs.shuidangran.top

TS:   s.split(",")
来源：http://znq.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://ozl.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ggb.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://zau.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nct.sweek.top

[E08] 数组按分隔符合并
来源：http://zis.316326.xyz

Py:   ",".join(items)
来源：http://pnj.zhengqikj.top

PHP:  implode(",", $items);
来源：http://amm.yj20258888.top

JS:   items.join(",")
来源：http://iqs.ehwqpu.com

TS:   items.join(",")
来源：http://tjp.tianlin.xyz

Java: String.join(",", items)
来源：http://omo.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://dsq.tianlin.xyz

Ruby: items.join(",")
来源：http://efw.nwbrower.top

C#:   string.Join(",", items)
来源：http://snt.bbcook.cn

[E09] 去除所有空白字符
来源：http://zxw.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ztq.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nmv.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://keh.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://yed.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://dfq.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eel.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dxq.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cfv.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://jga.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spp.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tau.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://per.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://afv.tian-w.cn

Java: String.format("%03d", 7)
来源：http://vwq.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qen.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yxy.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lum.yuxming.cn

[E11] 反转字符串
来源：http://aaq.jlsjyb.cn

Py:   s[::-1]
来源：http://jjc.yonumen.top

PHP:  strrev($s);
来源：http://icz.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://mei.cheryme.top

TS:   [...s].reverse().join("")
来源：http://oao.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://zuw.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://asm.ppjwa.cn

Ruby: s.reverse
来源：http://izl.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eko.yongpay.top

[E12] 统计某字符出现次数
来源：http://hdr.chenjidiqi.icu

Py:   s.count("a")
来源：http://gjg.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://ofk.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://lvu.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://pge.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mxu.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://mkx.pycfn.com

Ruby: s.count("a")
来源：http://tcw.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://aoi.jinqigufen.top

[E13] 逐字符遍历
来源：http://bkp.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://qwj.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://byd.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://gmd.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://plv.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lkv.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kfz.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qzh.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oge.yj202588.top

[E14] URL 编码与 Base64
来源：http://mqk.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fwt.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qvu.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://taz.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdx.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gyl.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rju.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vah.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qyv.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://wcq.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xkg.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fej.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jnx.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ghh.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rmv.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rcm.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pir.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fpi.jinqigfzy.top

[E16] 数字千分位
来源：http://ihq.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://rfx.havefunace.top

PHP:  number_format(1234567);
来源：http://vhy.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qyu.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://goi.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zeg.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vwz.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://csn.tanke756.top

C#:   1234567.ToString("N0")
来源：http://pqr.yfazqb.com

[E17] 首字母大写
来源：http://vyx.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kmb.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hkn.hnqzz.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sds.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ifj.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://chn.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kkw.jinqigfzy.top

Ruby: s.capitalize
来源：http://tus.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://otn.jinqigufen.top

[E18] 模板占位符替换
来源：http://icj.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lmo.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eqs.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tvs.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fma.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fos.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tvg.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sdg.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://owh.gzhubu.top

[E19] 多行文本按行拆分
来源：http://vjo.xylfe.cn

Py:   s.splitlines()
来源：http://vmu.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://frs.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://tcc.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://pen.birdmap.top

Java: s.lines().toList()
来源：http://dik.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://xkp.shanyushiyangkeji.top

Ruby: s.lines
来源：http://lpe.aibaodan.cn

C#:   s.Split('\n')
来源：http://qiu.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://dml.yongpay.top

Py:   if not s:
来源：http://for.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xoh.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gwv.andypj.xyz

TS:   if (s === "") {}
来源：http://usu.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://ezi.gaohongyu789.top

Go:   if s == "" {}
来源：http://rtq.chenzaomai.com

Ruby: if s.empty?
来源：http://kxg.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uzw.tarul.cn

[E21] 超长截断加省略号
来源：http://swf.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jig.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rew.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uak.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://chv.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sso.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://kdz.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ddy.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mmo.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://zwc.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xvm.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nkc.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjf.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://scs.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://djc.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cyh.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://fzb.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ccc.shuidangran.top

================================================================================
来源：http://wyp.jyoumei.cn

F. 文件与目录
来源：http://wxf.c1oappe.top

================================================================================
来源：http://gze.smart0.xyz

[F01] 读取整个文件
来源：http://ocj.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tsh.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://gfd.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://skh.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xxk.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://acg.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dju.c1oappe.top

Ruby: File.read("a.txt")
来源：http://yay.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vet.cashguo.top

[F02] 逐行读取文件
来源：http://puc.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qvm.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wbt.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wpt.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bak.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nxv.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://okz.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jjb.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://obl.yj202588.top

[F03] 写入文件（覆盖）
来源：http://rmy.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iji.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jlq.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ona.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzz.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://exo.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xep.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://yer.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ahq.guowangkeji.top

[F04] 追加写入文件
来源：http://mdk.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mdn.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ixs.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zkq.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrw.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://stk.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iiq.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ehh.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vwy.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://gnf.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xnj.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://mxs.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://zdr.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://aeb.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cau.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sdr.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://jer.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://yih.tian-w.cn

[F06] 删除文件
来源：http://yqm.sweek.top

Py:   os.remove("a.txt")
来源：http://vmo.aizwys.cn

PHP:  unlink("a.txt");
来源：http://nen.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rsu.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nim.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gmc.tanke756.top

Go:   os.Remove("a.txt")
来源：http://qis.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://mam.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://rzu.iojbl.cn

[F07] 创建目录（含多级）
来源：http://ftg.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cjt.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jlh.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eok.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rba.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qnt.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lnj.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwx.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zqc.ctjpmb.com

[F08] 遍历目录
来源：http://ekc.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wlu.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tvq.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://ruw.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://tdn.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ahn.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cty.52xcode.cn

Ruby: Dir.children("dir")
来源：http://rei.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://lye.gzhubu.top

[F09] 获取文件大小
来源：http://tzr.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://jzz.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://dpv.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://tcy.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://wnp.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://hkc.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bpv.yj20258.top

Ruby: File.size("a.txt")
来源：http://fjs.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://ret.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://yxk.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dwg.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zly.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hjq.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://tci.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wfq.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://exe.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dos.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kon.sufxvd.cn

[F11] 复制与移动文件
来源：http://oit.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kwg.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://irf.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asr.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dnz.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jlk.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vra.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yes.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hsf.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://jsd.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ivi.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rad.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tqs.tanke756.top

TS:   // 同上
来源：http://dsu.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ncz.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fcb.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ktl.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://brh.jiagoushi.top

================================================================================
来源：http://spu.ydjk.org.cn

G. 面向对象
来源：http://fah.yanxiufei.cn

================================================================================
来源：http://xtn.fengsongda.top

[G01] 定义类
来源：http://ghp.52xcode.cn

Py:   class User: pass
来源：http://qzw.sjlbkw.cn

PHP:  class User {}
来源：http://akt.jyoumei.cn

JS:   class User {}
来源：http://iwp.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://xhs.dianchejie.cn

Java: class User {}
来源：http://cuo.redwolf501.top

Go:   type User struct { Name string }
来源：http://ssz.hnqzz.top

Ruby: class User; end
来源：http://qwj.fanxiaobao.xyz

C#:   class User {}
来源：http://zoi.ywan-chungtsiang.top

[G02] 构造函数
来源：http://fup.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://jqn.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://eim.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://lee.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://zpl.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://hfu.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xsk.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://dps.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://pzk.zhaomingkeji.xyz

[G03] 实例属性
来源：http://dgu.iojbl.cn

Py:   self.name = "x"
来源：http://exw.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://tnb.dianchejie.cn

JS:   this.name = "x";
来源：http://esg.tianlin.xyz

TS:   name: string = "x";
来源：http://mjp.chenlongwang.top

Java: private String name;
来源：http://qgu.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uss.yongpay.top

Ruby: @name = "x"
来源：http://ofr.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://szu.sjlbkw.cn

[G04] 定义方法
来源：http://uvm.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://vsc.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tqf.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://ial.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://wth.tian-w.cn

Java: String greet() { return name; }
来源：http://xra.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uwt.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://nfp.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://drt.yonumen.top

[G05] 继承
来源：http://gjc.316326.xyz

Py:   class Admin(User): pass
来源：http://dbz.fzhhl.top

PHP:  class Admin extends User {}
来源：http://egm.tanke756.top

JS:   class Admin extends User {}
来源：http://owa.yj202588.top

TS:   class Admin extends User {}
来源：http://tif.hnqzz.top


<!-- 参考信息 -->