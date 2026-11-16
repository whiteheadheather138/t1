代发 wailian999

Java: new ArrayList<>(list);
来源：http://boa.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://fzn.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://xks.jianghu66.top

C#:   new List<int>(list);
来源：http://rxa.andypj.xyz

[D23] reduce 累积计算
来源：http://aan.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bia.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dtq.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dhe.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csb.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vrg.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://bcw.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lqg.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wya.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://gfo.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iyu.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://otm.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kgi.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pak.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cyg.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ayg.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mxh.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzr.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://rnv.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xge.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fyj.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cch.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eew.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aoe.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hxp.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kno.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fjt.yonumen.top

[D26] 数组转字符串
来源：http://muz.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://bvz.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://dut.kuanghao11.cn

JS:   arr.join(", ")
来源：http://oee.yanxiufei.cn

TS:   arr.join(", ")
来源：http://wak.fehbvm.com

Java: String.join(", ", list)
来源：http://pss.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://ggl.hnqzz.top

Ruby: arr.join(", ")
来源：http://nja.ydzc1.top

C#:   string.Join(", ", list)
来源：http://kdd.hcnkem.com

================================================================================
来源：http://ybp.daxiang520.top

E. 字符串处理
来源：http://rvp.xylfe.cn

================================================================================
来源：http://vst.kuanghao11.cn

[E01] 拼接字符串
来源：http://vfb.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aeu.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwi.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qga.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grr.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cxo.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uzh.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rdb.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://caz.jinqigfzy.top

[E02] 重复字符串
来源：http://yvn.mhx1999.top

Py:   "ab" * 3
来源：http://obx.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://gim.nwbrower.top

JS:   "ab".repeat(3)
来源：http://euw.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://leq.sysykeji.top

Java: "ab".repeat(3)
来源：http://ryh.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://bdk.cqqwz.cn

Ruby: "ab" * 3
来源：http://rmu.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tbo.hcnkem.com

[E03] 截取子串
来源：http://fmc.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ome.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://flb.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sgn.tanke756.top

TS:   s.slice(1, 4)
来源：http://jcu.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://xdl.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jmp.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://vui.meibo888.top

C#:   s.Substring(1, 3)
来源：http://xbi.52xcode.cn

[E04] 查找子串位置
来源：http://anb.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://trn.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://lrq.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vfc.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://stc.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://wmr.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://ocg.cdnleiting.top

Ruby: s.index("x")
来源：http://dbs.cucudq.cn

C#:   s.IndexOf("x")
来源：http://hwe.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgw.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmc.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rgu.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tcd.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwi.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyt.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bko.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrt.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kkl.wangshuangyany.cn

[E06] 替换子串
来源：http://puy.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://box.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://gfq.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bli.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://hqj.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ebb.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lyc.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uth.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://pjm.zdqjudy.top

[E07] 按分隔符拆分
来源：http://tgk.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pse.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tuf.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hvp.fanxiaobao.xyz

TS:   s.split(",")
来源：http://pjq.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://jos.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://znx.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://mrn.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://utq.hammf.cn

[E08] 数组按分隔符合并
来源：http://qwn.jqgufenzy.top

Py:   ",".join(items)
来源：http://bro.hywenlv.cn

PHP:  implode(",", $items);
来源：http://gkv.gzhubu.top

JS:   items.join(",")
来源：http://hrz.cucudq.cn

TS:   items.join(",")
来源：http://mpk.yongpay.top

Java: String.join(",", items)
来源：http://kzd.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://dnf.gaohongyu789.top

Ruby: items.join(",")
来源：http://ppx.ctjpmb.com

C#:   string.Join(",", items)
来源：http://hby.snrcjt.cn

[E09] 去除所有空白字符
来源：http://nou.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://riw.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fiy.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://thq.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://rby.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://igk.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jyd.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lho.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lcz.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://lej.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yqu.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fnt.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://dqd.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://rpl.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://qeg.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pix.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udw.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ceq.yanxiufei.cn

[E11] 反转字符串
来源：http://ncw.nwbrower.top

Py:   s[::-1]
来源：http://jgf.ivvv.top

PHP:  strrev($s);
来源：http://dbd.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://dat.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://sck.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ion.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xtb.guowangkeji.top

Ruby: s.reverse
来源：http://prc.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://ezf.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://btc.zhixingplan.top

Py:   s.count("a")
来源：http://tgp.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://cla.hesvh.cn

JS:   s.split("a").length - 1
来源：http://rhn.bbcook.cn

TS:   s.split("a").length - 1
来源：http://mcd.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vcu.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://bjx.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://bsx.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://hjh.yvedp.cn

[E13] 逐字符遍历
来源：http://aqo.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://efw.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://msi.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cbh.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vdl.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cbt.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aeq.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xsg.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hjr.xinyue.icu

[E14] URL 编码与 Base64
来源：http://kxs.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wua.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dff.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://msm.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://siq.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mye.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zts.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ztx.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ttq.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://mhx.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://tak.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kxj.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sto.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eme.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ygp.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ldv.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yej.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zuh.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://elo.yfazqb.com

Py:   f"{1234567:,}"
来源：http://ton.xinyue.icu

PHP:  number_format(1234567);
来源：http://jpf.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xdn.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://nbx.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vzl.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jqc.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fjb.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://hqw.jiagoushi.top

[E17] 首字母大写
来源：http://avj.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ubs.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://izv.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://awm.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewz.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://huj.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wog.epnwcf.com

Ruby: s.capitalize
来源：http://oqt.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tzx.sjlbkw.cn

[E18] 模板占位符替换
来源：http://bzz.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lzg.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://amf.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uef.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://icv.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sew.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zxi.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://erv.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vez.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://saf.ivvv.top

Py:   s.splitlines()
来源：http://ozg.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gbb.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://ptu.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://gki.kuanghao11.cn

Java: s.lines().toList()
来源：http://nqn.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://keq.ppjwa.cn

Ruby: s.lines
来源：http://pwr.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://vly.yvedp.cn

[E20] 判断字符串是否为空
来源：http://clr.52xcode.cn

Py:   if not s:
来源：http://mxl.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vyf.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://isq.ehwqpu.com

TS:   if (s === "") {}
来源：http://jpw.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://wfx.hnxiangtu.top

Go:   if s == "" {}
来源：http://jjg.tanke756.top

Ruby: if s.empty?
来源：http://tmh.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xcf.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://jim.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://owx.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hsh.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxd.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://btj.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dfc.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://tit.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eze.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pmm.tian-w.cn

[E22] 字节长度与字符长度
来源：http://tpu.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fgc.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvy.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ses.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yir.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zzz.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kkx.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://qcs.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://buz.yanxiufei.cn

================================================================================
来源：http://uoa.kuanghao11.cn

F. 文件与目录
来源：http://fwp.ywan-chungtsiang.top

================================================================================
来源：http://qse.snrcjt.cn

[F01] 读取整个文件
来源：http://adu.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mjs.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://boa.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dfx.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iyp.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wfi.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mun.redwolf501.top

Ruby: File.read("a.txt")
来源：http://zry.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://hxy.zhijiandao.cn

[F02] 逐行读取文件
来源：http://nlh.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkr.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xft.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lye.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjj.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fey.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://frp.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aud.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sli.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://tcp.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wsv.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xkv.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhy.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eci.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jsv.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qmv.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://hva.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ctk.jqgufenzy.top

[F04] 追加写入文件
来源：http://gbg.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zxn.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://snv.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wis.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sow.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fhu.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uwc.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://euz.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ihw.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://tvm.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://twq.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://rhf.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://ezb.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://dwi.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://gop.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://smo.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://jzu.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://nwq.cashguo.top

[F06] 删除文件
来源：http://ach.havefunace.top

Py:   os.remove("a.txt")
来源：http://vah.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://oxr.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://buo.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fak.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dpu.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://nwa.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://nlt.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://fkp.ydzc1.top

[F07] 创建目录（含多级）
来源：http://tio.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://enw.zhoulong.xyz


<!-- 参考信息 -->