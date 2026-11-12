代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xkp.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ija.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xdo.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://btc.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://onl.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cks.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://adz.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejs.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nyp.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wle.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ujt.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gov.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pel.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://duf.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cjr.bbcook.cn

[D26] 数组转字符串
来源：http://dmp.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://mfp.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://pab.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://swc.bbcook.cn

TS:   arr.join(", ")
来源：http://uxo.zhixingplan.top

Java: String.join(", ", list)
来源：http://mai.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://lyx.birdmap.top

Ruby: arr.join(", ")
来源：http://haq.yvedp.cn

C#:   string.Join(", ", list)
来源：http://dws.ppjwa.cn

================================================================================
来源：http://ikj.jqgfzy.top

E. 字符串处理
来源：http://ijo.hysaishi.cn

================================================================================
来源：http://exu.jyoumei.cn

[E01] 拼接字符串
来源：http://lhz.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cqd.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zyj.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cvx.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ite.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kes.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qup.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pat.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jug.vehdjk.com

[E02] 重复字符串
来源：http://giq.zycfv.cn

Py:   "ab" * 3
来源：http://mzh.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://ixn.ivvv.top

JS:   "ab".repeat(3)
来源：http://paq.fktsv.cn

TS:   "ab".repeat(3)
来源：http://evw.yuanzhike.top

Java: "ab".repeat(3)
来源：http://gud.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ayr.haohaochexian.top

Ruby: "ab" * 3
来源：http://fbf.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iya.hysaishi.cn

[E03] 截取子串
来源：http://fxr.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gez.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gsp.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zwn.yfazqb.com

TS:   s.slice(1, 4)
来源：http://hcj.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://qfl.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jui.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://mai.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://jhh.epnwcf.com

[E04] 查找子串位置
来源：http://myo.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://fdx.fzhhl.top

PHP:  strpos($s, "x");
来源：http://uul.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hfj.yj20258888.top

TS:   s.indexOf("x")
来源：http://idm.gzhubu.top

Java: s.indexOf("x")
来源：http://kel.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://mef.wangshuangyany.cn

Ruby: s.index("x")
来源：http://zyd.xuanzx.com

C#:   s.IndexOf("x")
来源：http://eab.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tqh.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cbe.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://een.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jrd.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jqa.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfn.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qdf.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fwp.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wrm.shangyingyoupin.top

[E06] 替换子串
来源：http://wya.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bat.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://zoz.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nln.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://kvp.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zdl.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://poq.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tjt.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://yjh.bjfxy.top

[E07] 按分隔符拆分
来源：http://kvi.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hqk.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://apc.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fsg.pycfn.com

TS:   s.split(",")
来源：http://kod.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://zxg.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://csa.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://jyk.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fxx.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://msz.tian-w.cn

Py:   ",".join(items)
来源：http://kop.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://fic.fktsv.cn

JS:   items.join(",")
来源：http://hcp.cdnleiting.top

TS:   items.join(",")
来源：http://qlw.feifeiyinyue.top

Java: String.join(",", items)
来源：http://lwh.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://wir.pycfn.com

Ruby: items.join(",")
来源：http://olr.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://mam.ehwqpu.com

[E09] 去除所有空白字符
来源：http://ziz.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ras.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://arj.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://xyj.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://dky.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://vnj.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mwg.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://aph.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hch.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://tgn.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fan.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pvl.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://gfr.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://fsx.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://rrk.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hbd.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjr.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oyx.cqqwz.cn

[E11] 反转字符串
来源：http://arq.jyoumei.cn

Py:   s[::-1]
来源：http://syr.yonumen.top

PHP:  strrev($s);
来源：http://gsd.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://ybl.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://ekn.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wtu.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mos.uphjek.com

Ruby: s.reverse
来源：http://xms.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xpn.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://ucy.hesvh.cn

Py:   s.count("a")
来源：http://mtj.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://oxy.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://lzy.ivvv.top

TS:   s.split("a").length - 1
来源：http://owv.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ddb.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://ght.c1oappe.top

Ruby: s.count("a")
来源：http://xpt.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://obs.zycfv.cn

[E13] 逐字符遍历
来源：http://pbt.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://hce.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pgj.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gpy.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oxh.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blx.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ots.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eev.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://izy.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://kfr.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ruv.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zrg.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://trg.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wqd.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kzs.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yrd.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sux.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://etl.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://rln.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ldt.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jov.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://duw.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fkk.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://obg.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jch.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqn.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ycd.svipenyu.cn

[E16] 数字千分位
来源：http://rlj.tanke756.top

Py:   f"{1234567:,}"
来源：http://jsr.zhixingplan.top

PHP:  number_format(1234567);
来源：http://jxr.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ele.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bqf.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://whq.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qlv.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hqf.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://pno.hnxiangtu.top

[E17] 首字母大写
来源：http://bcx.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ape.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jhv.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ldp.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sib.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mvh.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hbz.yongpay.top

Ruby: s.capitalize
来源：http://sbi.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nrk.cucudq.cn

[E18] 模板占位符替换
来源：http://adj.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://avy.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fbc.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gil.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://sck.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tin.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tkc.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eta.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qls.redwolf501.top

[E19] 多行文本按行拆分
来源：http://cto.havefunace.top

Py:   s.splitlines()
来源：http://jck.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qkf.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://ytf.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://sai.sxryk.cn

Java: s.lines().toList()
来源：http://dar.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://fik.tian-w.cn

Ruby: s.lines
来源：http://fgz.yongpay.top

C#:   s.Split('\n')
来源：http://sjf.fehbvm.com

[E20] 判断字符串是否为空
来源：http://nxs.cdnleiting.top

Py:   if not s:
来源：http://tuv.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpy.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nnh.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://wym.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://lry.daxiang520.top

Go:   if s == "" {}
来源：http://fti.shuidangran.top

Ruby: if s.empty?
来源：http://txr.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dmg.bbcook.cn

[E21] 超长截断加省略号
来源：http://hmy.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dui.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ooo.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fni.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jso.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yon.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://dti.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mni.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wna.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://htg.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zve.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mjw.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekk.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kbr.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eaq.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jts.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://oho.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xew.gogol.net.cn

================================================================================
来源：http://sth.ydjk.org.cn

F. 文件与目录
来源：http://ciu.quarkkingdee.top

================================================================================
来源：http://mjt.bjfxy.top

[F01] 读取整个文件
来源：http://eat.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hhu.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://bln.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lbb.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jit.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dms.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nkm.fktsv.cn

Ruby: File.read("a.txt")
来源：http://log.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://odl.fengsongda.top

[F02] 逐行读取文件
来源：http://ksi.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wkr.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ula.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jnm.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://neo.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cco.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vtc.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bpd.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cji.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://pao.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yaf.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ebk.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://amc.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aih.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfl.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wcu.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://dmj.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bju.zhijiandao.cn

[F04] 追加写入文件
来源：http://ama.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzf.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fli.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nut.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jaa.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ilu.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://skr.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kpm.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://prp.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://zqo.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vpp.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://sej.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://gls.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://vtv.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bkw.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eyu.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://vol.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://fvw.fengsongda.top

[F06] 删除文件
来源：http://bfa.mhx1999.top

Py:   os.remove("a.txt")
来源：http://ubi.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://ydg.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://cjm.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://xlm.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ifn.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://tve.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://iji.ivvv.top

C#:   File.Delete("a.txt");
来源：http://zty.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://lne.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xfy.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aae.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndg.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jaf.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mkr.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyv.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ucv.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kbz.guannengcc.top

[F08] 遍历目录
来源：http://tap.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zoo.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wmj.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://ekb.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://mvb.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdd.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zpb.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://oej.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://ydx.yfazqb.com


<!-- 参考信息 -->