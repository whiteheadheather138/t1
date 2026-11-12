代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thp.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://wcb.chenjidiqi.icu

Go:   // 手写循环
来源：http://ttq.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nsy.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gve.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://nho.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vpf.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fqo.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fyw.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vgc.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uod.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kpo.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kca.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tsz.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://pum.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dmx.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uod.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tqs.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wrx.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pdm.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iqw.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vhd.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://drj.xylfe.cn

[D26] 数组转字符串
来源：http://clo.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://vix.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://fvm.chenlongwang.top

JS:   arr.join(", ")
来源：http://nqn.shzxlz.cn

TS:   arr.join(", ")
来源：http://dcw.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://kpm.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://qmo.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://pta.fengsongda.top

C#:   string.Join(", ", list)
来源：http://auy.sxryk.cn

================================================================================
来源：http://aof.zhijiandao.cn

E. 字符串处理
来源：http://uib.yj20258.top

================================================================================
来源：http://gkj.iojbl.cn

[E01] 拼接字符串
来源：http://sgk.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ofp.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpv.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofm.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cce.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kic.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yud.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hdr.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vdi.yvedp.cn

[E02] 重复字符串
来源：http://vhv.hcnkem.com

Py:   "ab" * 3
来源：http://gum.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://osk.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://vik.epnwcf.com

TS:   "ab".repeat(3)
来源：http://ldd.bjfxy.top

Java: "ab".repeat(3)
来源：http://rsn.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://vfe.zhijiandao.cn

Ruby: "ab" * 3
来源：http://mop.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwt.hcnkem.com

[E03] 截取子串
来源：http://ydq.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://igb.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dby.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hhg.cashguo.top

TS:   s.slice(1, 4)
来源：http://qfp.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://xor.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ifh.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wtu.birdmap.top

C#:   s.Substring(1, 3)
来源：http://ieu.jiagoushi.top

[E04] 查找子串位置
来源：http://dou.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://wli.yvedp.cn

PHP:  strpos($s, "x");
来源：http://bwq.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jof.c1oappe.top

TS:   s.indexOf("x")
来源：http://lxp.fengsongda.top

Java: s.indexOf("x")
来源：http://bmo.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://sfv.yonumen.top

Ruby: s.index("x")
来源：http://idd.yuxming.cn

C#:   s.IndexOf("x")
来源：http://ehn.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zch.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aet.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nnw.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://flf.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cny.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxp.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fbx.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lyx.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mog.xinyue.icu

[E06] 替换子串
来源：http://sow.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ekc.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://vvp.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgj.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://lxj.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ecj.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vzv.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ujg.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://jwj.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://bwv.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jhu.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ulm.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wcq.zdbjq.cn

TS:   s.split(",")
来源：http://wfb.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://jdl.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vjk.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://ysw.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://adi.vehdjk.com

[E08] 数组按分隔符合并
来源：http://xgv.vqdsnc.cn

Py:   ",".join(items)
来源：http://kxp.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://uhc.tian-w.cn

JS:   items.join(",")
来源：http://bzd.yvedp.cn

TS:   items.join(",")
来源：http://qcy.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://raq.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://azk.tarul.cn

Ruby: items.join(",")
来源：http://mfc.jinqigufen.top

C#:   string.Join(",", items)
来源：http://oob.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://jax.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fhf.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gcb.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://ivn.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://lnz.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://srj.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tkz.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dyy.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jvp.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://pji.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wam.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://etu.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://rft.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://yqk.yj20258888.top

Java: String.format("%03d", 7)
来源：http://eyl.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gki.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jui.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gdr.jinqigufen.top

[E11] 反转字符串
来源：http://qln.dashuyun.cn

Py:   s[::-1]
来源：http://adn.yonumen.top

PHP:  strrev($s);
来源：http://vcj.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://tnq.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://sxm.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zgk.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dpx.tianlin.xyz

Ruby: s.reverse
来源：http://euh.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kbm.zycfv.cn

[E12] 统计某字符出现次数
来源：http://oxj.redwolf501.top

Py:   s.count("a")
来源：http://yzu.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://ugm.xinyue.icu

JS:   s.split("a").length - 1
来源：http://nji.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://bxk.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lqt.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://gzb.9152youxi.cn

Ruby: s.count("a")
来源：http://ont.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://xvq.yuanzhike.top

[E13] 逐字符遍历
来源：http://dhe.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://igv.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmq.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ceb.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxq.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nqn.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gza.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wbn.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gwo.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://mfc.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lqp.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zfi.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://con.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iwy.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pwg.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://exd.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blq.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bpo.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://nwp.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sjd.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axn.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qtd.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ndk.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qfg.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://woz.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjt.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qjx.cqqwz.cn

[E16] 数字千分位
来源：http://yyu.xylfe.cn

Py:   f"{1234567:,}"
来源：http://wab.dianchejie.cn

PHP:  number_format(1234567);
来源：http://nas.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rbh.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://iyc.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://edz.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xfq.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqs.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://sai.yanxiufei.cn

[E17] 首字母大写
来源：http://opn.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kbu.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://txk.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jtb.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzj.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eau.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://igx.sweek.top

Ruby: s.capitalize
来源：http://cms.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nzg.fktsv.cn

[E18] 模板占位符替换
来源：http://fsk.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ghd.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dar.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wsd.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zgp.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kte.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zvv.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ymc.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqv.guannengcc.top

[E19] 多行文本按行拆分
来源：http://rvm.9152youxi.cn

Py:   s.splitlines()
来源：http://iqc.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ivy.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://icy.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://tgf.yuanzhike.top

Java: s.lines().toList()
来源：http://mzo.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://uqh.nanxuanxn.top

Ruby: s.lines
来源：http://mbd.zdbjq.cn

C#:   s.Split('\n')
来源：http://swg.yongpay.top

[E20] 判断字符串是否为空
来源：http://kit.zhaomingkeji.xyz

Py:   if not s:
来源：http://vob.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mcp.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://udo.chenzaomai.com

TS:   if (s === "") {}
来源：http://vdm.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://gqg.hysaishi.cn

Go:   if s == "" {}
来源：http://wzb.guowangkeji.top

Ruby: if s.empty?
来源：http://dlg.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vmd.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://szb.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qix.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://amz.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hmo.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oev.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://izq.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://qjo.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hro.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ngv.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://sjk.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tjr.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exr.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ztr.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://miz.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mlw.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hch.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://wfs.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aur.ehwqpu.com

================================================================================
来源：http://vgi.ywan-chungtsiang.top

F. 文件与目录
来源：http://pef.pengpengdd.cyou

================================================================================
来源：http://unt.jqgfzy.top

[F01] 读取整个文件
来源：http://iqh.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jim.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://soj.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xym.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://one.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pws.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jug.aizwys.cn

Ruby: File.read("a.txt")
来源：http://zjn.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://mdn.ehwqpu.com

[F02] 逐行读取文件
来源：http://ezh.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lbg.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eub.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilc.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://brf.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hcc.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hkn.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rgh.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tvw.birdmap.top

[F03] 写入文件（覆盖）
来源：http://ptv.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ger.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ixd.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hsk.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kmf.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pyd.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://guu.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qnw.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyf.andypj.xyz

[F04] 追加写入文件
来源：http://yzj.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fll.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vys.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nzx.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dnh.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vyl.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vqs.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vra.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxm.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://yue.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xad.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://imy.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://gsv.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://ieh.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yuh.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qrf.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://aae.cheryme.top

C#:   File.Exists("a.txt")
来源：http://oie.feifeiyinyue.top

[F06] 删除文件
来源：http://hry.cashguo.top

Py:   os.remove("a.txt")
来源：http://npl.bjfxy.top

PHP:  unlink("a.txt");
来源：http://xnv.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cgm.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://daq.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rgu.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://pue.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://oew.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://nxu.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://cqu.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fnk.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lro.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fas.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hok.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://byr.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rss.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mko.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oup.sweek.top

[F08] 遍历目录
来源：http://sfp.sufxvd.cn


<!-- 参考信息 -->