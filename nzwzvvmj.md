代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pxj.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ewr.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qzm.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ndy.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nzt.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://acn.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://poh.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wsn.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uhy.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jjo.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aic.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jrx.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://elb.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uuh.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tnx.dianchejie.cn

[D26] 数组转字符串
来源：http://eov.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://zoq.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://mhc.cqqwz.cn

JS:   arr.join(", ")
来源：http://xap.iojbl.cn

TS:   arr.join(", ")
来源：http://gck.guowangkeji.top

Java: String.join(", ", list)
来源：http://hzo.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://fzs.tarul.cn

Ruby: arr.join(", ")
来源：http://uii.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://wae.sysykeji.top

================================================================================
来源：http://lir.xuetiantiany.cn

E. 字符串处理
来源：http://tos.yj20258888.top

================================================================================
来源：http://xwk.zhijiandao.cn

[E01] 拼接字符串
来源：http://pyr.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gnp.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nvg.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cgp.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajf.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kkl.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jwm.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iml.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://txt.gzhubu.top

[E02] 重复字符串
来源：http://kys.birdmap.top

Py:   "ab" * 3
来源：http://wbg.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://asf.tarul.cn

JS:   "ab".repeat(3)
来源：http://wtt.yongpay.top

TS:   "ab".repeat(3)
来源：http://ckp.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://cjq.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://okv.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://rrc.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hqj.yj202588.top

[E03] 截取子串
来源：http://vuq.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sqk.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://faz.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eas.yfazqb.com

TS:   s.slice(1, 4)
来源：http://ovr.epnwcf.com

Java: s.substring(1, 4)
来源：http://abo.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aih.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pxx.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://igd.ivvv.top

[E04] 查找子串位置
来源：http://lvt.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://jfm.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://xym.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jse.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://hsq.9152youxi.cn

Java: s.indexOf("x")
来源：http://rkc.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://igu.smart0.xyz

Ruby: s.index("x")
来源：http://irn.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://hmo.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijy.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ror.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kch.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://njt.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bkx.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mvd.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gpb.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mfs.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wgl.yfazqb.com

[E06] 替换子串
来源：http://rtv.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qdy.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://cxs.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dnz.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://zuv.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ofj.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tbp.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cqr.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://bdr.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://ugm.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yky.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://teq.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lsz.shangyingyoupin.top

TS:   s.split(",")
来源：http://gng.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://paq.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://trm.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://ort.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qga.xziqi.cn

[E08] 数组按分隔符合并
来源：http://msi.sysykeji.top

Py:   ",".join(items)
来源：http://utr.hesvh.cn

PHP:  implode(",", $items);
来源：http://tev.yj20258.top

JS:   items.join(",")
来源：http://iqi.yonumen.top

TS:   items.join(",")
来源：http://ant.xinyue.icu

Java: String.join(",", items)
来源：http://jna.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://gjd.chenlongwang.top

Ruby: items.join(",")
来源：http://tdz.zhaomingkeji.xyz

C#:   string.Join(",", items)
来源：http://atk.yj202588.top

[E09] 去除所有空白字符
来源：http://mey.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fhp.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pto.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://ymr.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://frv.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://stv.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oes.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lbv.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ihf.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://ogo.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://waa.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ppj.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://hto.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://kia.yongpay.top

Java: String.format("%03d", 7)
来源：http://jjr.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://umj.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ier.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sui.daria6918.cn

[E11] 反转字符串
来源：http://vuy.jqgfzy.top

Py:   s[::-1]
来源：http://wso.hnxiangtu.top

PHP:  strrev($s);
来源：http://vyj.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://izu.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://rpn.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pan.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://naj.gzhubu.top

Ruby: s.reverse
来源：http://bnd.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gxp.0kj1m.cn

[E12] 统计某字符出现次数
来源：http://rhs.hfpthk.cn

Py:   s.count("a")
来源：http://ugm.ivvv.top

PHP:  substr_count($s, "a");
来源：http://jwg.guannengcc.top

JS:   s.split("a").length - 1
来源：http://uae.guannengcc.top

TS:   s.split("a").length - 1
来源：http://rob.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qbf.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://fib.quarkkingdee.top

Ruby: s.count("a")
来源：http://sfe.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://szh.daria6918.cn

[E13] 逐字符遍历
来源：http://kgl.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://inh.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ldi.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exd.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://wvo.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tjv.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zbb.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bqb.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://adt.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://qyy.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lba.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nqj.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tkp.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdf.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ubh.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://brl.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rmc.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bdh.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://hpr.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mfw.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zcw.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://krs.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dju.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wjz.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dmq.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mck.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pbz.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://tpw.xylfe.cn

Py:   f"{1234567:,}"
来源：http://eva.shuidangran.top

PHP:  number_format(1234567);
来源：http://zfp.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zga.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kwm.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rea.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qoo.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhn.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://vdx.yongpay.top

[E17] 首字母大写
来源：http://ear.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ozt.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ejy.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bai.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://use.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uds.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ssh.fktsv.cn

Ruby: s.capitalize
来源：http://eqq.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qqs.chenlongwang.top

[E18] 模板占位符替换
来源：http://gez.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ycp.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbv.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ctm.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://adp.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oob.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ohh.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ilw.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tkk.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://lii.hysaishi.cn

Py:   s.splitlines()
来源：http://tzr.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zjd.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://afy.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://wzd.chenjidiqi.icu

Java: s.lines().toList()
来源：http://ezp.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://olm.ppjwa.cn

Ruby: s.lines
来源：http://koh.yvedp.cn

C#:   s.Split('\n')
来源：http://cuv.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://luf.shanyushiyangkeji.top

Py:   if not s:
来源：http://rgm.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ioh.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hub.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://mph.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://lby.gotoacloud.top

Go:   if s == "" {}
来源：http://klq.daria6918.cn

Ruby: if s.empty?
来源：http://nnk.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pri.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://lhu.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://chu.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iok.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ewu.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qtg.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hyv.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://gkw.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nvv.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cci.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://uno.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://trb.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nfz.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fif.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tdb.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dww.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tcy.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://lax.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjo.ivvv.top

================================================================================
来源：http://udy.yfazqb.com

F. 文件与目录
来源：http://hqe.svipenyu.cn

================================================================================
来源：http://lws.jqgfzy.top

[F01] 读取整个文件
来源：http://dbn.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rcl.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://eze.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qkd.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eff.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qnh.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hph.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://apl.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://oae.daria6918.cn

[F02] 逐行读取文件
来源：http://hwd.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lyx.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tqo.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://epu.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qda.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jgg.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ykz.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yex.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmo.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://vcq.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qgi.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lmj.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzt.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akk.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hhw.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://udy.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://rsj.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zps.cqqwz.cn

[F04] 追加写入文件
来源：http://bsw.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mme.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xfa.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtl.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjo.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bia.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vpl.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ahc.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nma.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://lbl.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yed.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://gnq.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://fql.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://uxs.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://khu.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://syj.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://uss.sweek.top

C#:   File.Exists("a.txt")
来源：http://ysp.cheryme.top

[F06] 删除文件
来源：http://tik.tanke756.top

Py:   os.remove("a.txt")
来源：http://sgz.cashguo.top

PHP:  unlink("a.txt");
来源：http://epj.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hav.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://amz.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cje.birdmap.top

Go:   os.Remove("a.txt")
来源：http://uyv.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://glh.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://ufr.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://nwa.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mqb.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jax.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://smh.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khp.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wns.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://keg.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://huy.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gam.bbcook.cn

[F08] 遍历目录
来源：http://avx.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://upg.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpj.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://ukw.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://cta.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ipc.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://azw.vehdjk.com

Ruby: Dir.children("dir")
来源：http://mzg.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://mlx.daxiang520.top


<!-- 参考信息 -->