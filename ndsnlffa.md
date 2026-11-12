代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tpg.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://evh.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cif.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kdo.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wir.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tnx.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nvn.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nyj.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ddk.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wjq.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://ayx.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bou.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rwm.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sqg.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xco.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://spb.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gga.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wny.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zmr.tarul.cn

[D26] 数组转字符串
来源：http://kzp.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://drg.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://ofk.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://zuy.hammf.cn

TS:   arr.join(", ")
来源：http://lyq.guowangkeji.top

Java: String.join(", ", list)
来源：http://kww.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://mgj.cucudq.cn

Ruby: arr.join(", ")
来源：http://dpq.sweek.top

C#:   string.Join(", ", list)
来源：http://rdd.zdqjudy.top

================================================================================
来源：http://vmn.hfpthk.cn

E. 字符串处理
来源：http://cqi.ppjwa.cn

================================================================================
来源：http://tuh.feifeiyinyue.top

[E01] 拼接字符串
来源：http://rse.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gek.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cgj.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eyo.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtv.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dmb.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mqq.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://teg.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xnv.bbcook.cn

[E02] 重复字符串
来源：http://nms.yuanzhike.top

Py:   "ab" * 3
来源：http://jiw.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://jnb.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://fwi.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://ueh.chenlongwang.top

Java: "ab".repeat(3)
来源：http://dhj.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://iiu.chenlongwang.top

Ruby: "ab" * 3
来源：http://ipz.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dhh.havefunace.top

[E03] 截取子串
来源：http://uyw.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozv.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://piu.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikv.xinyue.icu

TS:   s.slice(1, 4)
来源：http://owm.jiagoushi.top

Java: s.substring(1, 4)
来源：http://iyq.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sid.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://uxt.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://ypg.xuanzx.com

[E04] 查找子串位置
来源：http://lel.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://soj.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://ftf.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gce.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://ifp.yuxming.cn

Java: s.indexOf("x")
来源：http://tll.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://gwh.tian-w.cn

Ruby: s.index("x")
来源：http://xft.andypj.xyz

C#:   s.IndexOf("x")
来源：http://onj.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qgi.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jxf.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ala.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://idp.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eit.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lul.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ify.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xph.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqi.guannengcc.top

[E06] 替换子串
来源：http://xgo.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aib.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://gyw.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqr.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://dyy.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxn.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cto.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzu.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://hbs.sweek.top

[E07] 按分隔符拆分
来源：http://szt.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ynn.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpo.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pib.cashguo.top

TS:   s.split(",")
来源：http://yqk.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://rmp.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://god.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://kzh.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mrg.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://ips.bjfxy.top

Py:   ",".join(items)
来源：http://jah.haohaochexian.top

PHP:  implode(",", $items);
来源：http://bcw.tian-w.cn

JS:   items.join(",")
来源：http://rpr.nanxuanxn.top

TS:   items.join(",")
来源：http://bxz.yfazqb.com

Java: String.join(",", items)
来源：http://lco.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://qbs.chenlongwang.top

Ruby: items.join(",")
来源：http://mhb.jinqigufen.top

C#:   string.Join(",", items)
来源：http://ute.yfazqb.com

[E09] 去除所有空白字符
来源：http://hnm.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hsc.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uab.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://kjv.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://qjv.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://msz.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://asf.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bkg.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hdz.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://fpk.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://icc.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xkp.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://xsy.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://jgs.daria6918.cn

Java: String.format("%03d", 7)
来源：http://qsq.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hnx.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://icn.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fzd.tianlin.xyz

[E11] 反转字符串
来源：http://lza.cdnleiting.top

Py:   s[::-1]
来源：http://xzi.gotoacloud.top

PHP:  strrev($s);
来源：http://yiw.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://fxa.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://zmd.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jro.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fbs.hesvh.cn

Ruby: s.reverse
来源：http://qaq.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://vxg.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://jeb.yj202588.top

Py:   s.count("a")
来源：http://eth.birdmap.top

PHP:  substr_count($s, "a");
来源：http://ztc.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://tfh.52xcode.cn

TS:   s.split("a").length - 1
来源：http://zpf.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jab.sweek.top

Go:   strings.Count(s, "a")
来源：http://hkt.shzxlz.cn

Ruby: s.count("a")
来源：http://dtg.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://uft.hammf.cn

[E13] 逐字符遍历
来源：http://fjd.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://ozy.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://anx.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jaj.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zzv.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hlz.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mce.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ilf.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nww.iojbl.cn

[E14] URL 编码与 Base64
来源：http://jnl.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yxi.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://srz.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kwx.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://inh.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lrc.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jkx.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://krv.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://szn.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://tzu.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nfd.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xdf.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pbs.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yas.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yzw.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lcm.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hoz.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pcn.dianchejie.cn

[E16] 数字千分位
来源：http://lgm.guannengcc.top

Py:   f"{1234567:,}"
来源：http://nli.ivvv.top

PHP:  number_format(1234567);
来源：http://vun.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wgl.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ytd.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cmz.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wpp.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pfx.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://nbk.gaohongyu789.top

[E17] 首字母大写
来源：http://jja.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cjr.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nek.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpt.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tnc.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wit.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nfy.andypj.xyz

Ruby: s.capitalize
来源：http://xqj.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ftc.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://wgf.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hzi.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sga.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zue.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://siz.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dtb.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iru.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tbd.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xws.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://vfc.yvedp.cn

Py:   s.splitlines()
来源：http://hko.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://avn.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://apn.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://obo.xylfe.cn

Java: s.lines().toList()
来源：http://efn.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://sjv.tanke756.top

Ruby: s.lines
来源：http://xou.52xcode.cn

C#:   s.Split('\n')
来源：http://kwa.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://ipe.cucudq.cn

Py:   if not s:
来源：http://osf.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jno.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://btb.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://ldr.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://voc.nanxinkj.top

Go:   if s == "" {}
来源：http://iyx.xylfe.cn

Ruby: if s.empty?
来源：http://tcl.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vdo.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://kby.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jvr.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vvu.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwx.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mag.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uph.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://kwx.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sun.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aik.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ces.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vcx.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olx.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvh.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wlv.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ntp.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pvo.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://ypg.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vsz.hysaishi.cn

================================================================================
来源：http://alf.xinyue.icu

F. 文件与目录
来源：http://pkx.zhengqikj.top

================================================================================
来源：http://mlh.316326.xyz

[F01] 读取整个文件
来源：http://nir.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wtu.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://zle.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzi.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uyh.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://opt.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sqn.c1oappe.top

Ruby: File.read("a.txt")
来源：http://gyz.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jkq.tianlin.xyz

[F02] 逐行读取文件
来源：http://vah.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://max.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://opi.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jan.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://saj.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sxb.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://znq.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hem.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mbg.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://fuq.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gdk.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://uyv.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfg.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bqx.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ndo.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jdx.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://ckn.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrf.chenlongwang.top

[F04] 追加写入文件
来源：http://taa.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yiu.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qzb.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://epb.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejl.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rdz.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yzl.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://szh.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://foe.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://lse.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hww.birdmap.top

PHP:  file_exists("a.txt");
来源：http://opq.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://cpm.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://oao.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mip.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yvd.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://pah.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://ung.yonumen.top

[F06] 删除文件
来源：http://ksn.ybcxt.top

Py:   os.remove("a.txt")
来源：http://nig.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://bez.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://eql.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zia.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xtq.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://kzl.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://ogw.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://csm.yongpay.top

[F07] 创建目录（含多级）
来源：http://isi.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rts.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lrz.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zdm.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ouf.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vsw.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mbh.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocj.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://edb.c1oappe.top

[F08] 遍历目录
来源：http://wrh.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iof.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cxr.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://lcv.sweek.top

TS:   fs.readdirSync("dir")
来源：http://fkt.xinyue.icu


<!-- 参考信息 -->