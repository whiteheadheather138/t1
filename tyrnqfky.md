代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://voq.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wno.daxiang520.top

Go:   // 手写循环
来源：http://xcb.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xou.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ccz.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://unc.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ghh.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rdc.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://prr.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tbv.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xhu.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lur.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bwq.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyj.havefunace.top

[D25] Set 集合去重与交并差
来源：http://phj.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lta.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ajc.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://llv.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wgj.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dib.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cdx.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gny.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://smp.nwbrower.top

[D26] 数组转字符串
来源：http://jdg.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://vzv.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://hme.yj20258.top

JS:   arr.join(", ")
来源：http://yud.nanxuanxn.top

TS:   arr.join(", ")
来源：http://ysj.hnxiangtu.top

Java: String.join(", ", list)
来源：http://nux.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://cnl.hywenlv.cn

Ruby: arr.join(", ")
来源：http://afe.bjfxy.top

C#:   string.Join(", ", list)
来源：http://dsc.andypj.xyz

================================================================================
来源：http://zwc.316326.xyz

E. 字符串处理
来源：http://mjg.zhixingplan.top

================================================================================
来源：http://ruo.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://ebv.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qdo.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://noj.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://drn.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vvm.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ttn.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bkr.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mjd.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pxh.wangdashe.top

[E02] 重复字符串
来源：http://iaf.sysykeji.top

Py:   "ab" * 3
来源：http://qjg.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://kum.yonumen.top

JS:   "ab".repeat(3)
来源：http://bqo.redwolf501.top

TS:   "ab".repeat(3)
来源：http://xld.yj202588.top

Java: "ab".repeat(3)
来源：http://cne.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://yta.zhengqikj.top

Ruby: "ab" * 3
来源：http://jcr.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eoa.jinyuanbaomall.cn

[E03] 截取子串
来源：http://oja.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rvm.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xey.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvv.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://otk.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://inc.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://myh.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://btn.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://dax.gogol.net.cn

[E04] 查找子串位置
来源：http://eto.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://myr.fengsongda.top

PHP:  strpos($s, "x");
来源：http://zsj.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://did.sufxvd.cn

TS:   s.indexOf("x")
来源：http://ljx.zhengqikj.top

Java: s.indexOf("x")
来源：http://ppb.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://tnj.nwbrower.top

Ruby: s.index("x")
来源：http://oeq.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://lhh.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ujb.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zsi.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://odu.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuc.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpw.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ksy.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ocp.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ryk.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hss.jqgfzy.top

[E06] 替换子串
来源：http://lju.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xkb.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://amr.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhb.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://pcf.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdm.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qiz.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wqg.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://qev.zdbjq.cn

[E07] 按分隔符拆分
来源：http://juh.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://let.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exe.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xqr.tarul.cn

TS:   s.split(",")
来源：http://kie.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://abe.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lvd.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://wko.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fef.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://ote.shuidangran.top

Py:   ",".join(items)
来源：http://kzk.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://gyl.mhx1999.top

JS:   items.join(",")
来源：http://oci.ybcxt.top

TS:   items.join(",")
来源：http://iga.guannengcc.top

Java: String.join(",", items)
来源：http://voa.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://cyh.0kj1m.cn

Ruby: items.join(",")
来源：http://szj.0kj1m.cn

C#:   string.Join(",", items)
来源：http://twc.fktsv.cn

[E09] 去除所有空白字符
来源：http://zar.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bai.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://non.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://szs.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://evr.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://omf.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xqr.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://neq.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ume.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://dyu.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wal.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ufk.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://idn.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://ybz.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://ctk.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hlg.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hwv.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://esi.ybcxt.top

[E11] 反转字符串
来源：http://avx.zhoulong.xyz

Py:   s[::-1]
来源：http://cdu.svipenyu.cn

PHP:  strrev($s);
来源：http://vrb.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://yap.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://hcf.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mfo.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cyo.chenzaomai.com

Ruby: s.reverse
来源：http://ito.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xnl.redwolf501.top

[E12] 统计某字符出现次数
来源：http://adq.feifeiyinyue.top

Py:   s.count("a")
来源：http://rtm.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://xsw.epnwcf.com

JS:   s.split("a").length - 1
来源：http://atm.yj20258.top

TS:   s.split("a").length - 1
来源：http://jaz.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oxu.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://flr.52xcode.cn

Ruby: s.count("a")
来源：http://bss.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://rix.yanxiufei.cn

[E13] 逐字符遍历
来源：http://gxf.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://anq.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mig.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ziy.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pll.nwbrower.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rfx.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dgk.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uti.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vih.hcnkem.com

[E14] URL 编码与 Base64
来源：http://iei.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uvq.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pah.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://olm.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jli.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bdj.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qwc.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xgu.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jls.feifeiyinyue.top

[E15] HTML 转义 / 反转义
来源：http://aoo.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zby.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://duq.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cue.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hlr.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tvj.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jqw.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uzg.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://exb.jqgfzy.top

[E16] 数字千分位
来源：http://gkb.yongpay.top

Py:   f"{1234567:,}"
来源：http://ylv.ydzc1.top

PHP:  number_format(1234567);
来源：http://jid.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ljb.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://smc.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ury.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iqf.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://riw.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://efe.sweek.top

[E17] 首字母大写
来源：http://cli.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hzk.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnm.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ryy.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spj.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blh.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://abu.jianghu66.top

Ruby: s.capitalize
来源：http://swz.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dlm.zhijiandao.cn

[E18] 模板占位符替换
来源：http://izm.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nqt.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gsz.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hht.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ubn.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nud.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bld.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dot.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://azf.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://jtj.ydzc1.top

Py:   s.splitlines()
来源：http://vjj.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xtz.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://ywd.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://siy.52xcode.cn

Java: s.lines().toList()
来源：http://utq.sweek.top

Go:   strings.Split(s, "\n")
来源：http://esq.hesvh.cn

Ruby: s.lines
来源：http://btg.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://nom.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://cbr.hcnkem.com

Py:   if not s:
来源：http://xhb.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xka.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kbb.ehwqpu.com

TS:   if (s === "") {}
来源：http://hnk.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://vmt.hongshengwenyu.top

Go:   if s == "" {}
来源：http://rkr.gotoacloud.top

Ruby: if s.empty?
来源：http://oor.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://peb.zhixingplan.top

[E21] 超长截断加省略号
来源：http://veh.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bpe.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mmr.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vff.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yjl.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yai.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://rxk.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ndd.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qin.wangdashe.top

[E22] 字节长度与字符长度
来源：http://kkc.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ems.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlx.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zrd.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qfj.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rpk.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bjb.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://sld.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xlq.tianlin.xyz

================================================================================
来源：http://ame.yonumen.top

F. 文件与目录
来源：http://cfm.yj202588.top

================================================================================
来源：http://goz.gotoacloud.top

[F01] 读取整个文件
来源：http://fjb.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xst.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://vvp.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://waw.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywf.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ciz.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://piu.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://unz.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://euk.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://kpe.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctd.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://exb.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dej.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hot.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uow.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cnm.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rwy.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kkh.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://jkz.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpw.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dvq.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xdd.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifm.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vdn.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hbs.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://vnu.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://psm.jiagoushi.top

[F04] 追加写入文件
来源：http://nql.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rzh.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://quu.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://med.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fok.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fzo.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sah.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://osl.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://apg.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://lta.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oar.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://noo.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://wyg.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://ciz.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zje.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jrf.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://rtg.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://xos.aizwys.cn

[F06] 删除文件
来源：http://clm.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://vfi.fzhhl.top

PHP:  unlink("a.txt");
来源：http://sqp.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://ehm.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cvj.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ltp.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://nsv.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://ima.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://dqf.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://vsn.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eaf.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aoy.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mcu.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rmq.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://asl.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ema.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://knd.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ykr.jqgufenzy.top

[F08] 遍历目录
来源：http://lgt.hnxiangtu.top


<!-- 参考信息 -->