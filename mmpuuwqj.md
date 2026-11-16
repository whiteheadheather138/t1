代发 wailian999

Java: new ArrayList<>(list);
来源：http://kae.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://zco.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://zog.sxryk.cn

C#:   new List<int>(list);
来源：http://xkt.cdnleiting.top

[D23] reduce 累积计算
来源：http://qmn.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://onu.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ozt.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gkl.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pue.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://slx.yuxming.cn

Go:   // 手写循环
来源：http://lme.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cad.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://enq.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://vgv.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lvl.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfk.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xon.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://txl.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kjl.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cee.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lvp.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mau.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://iek.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sqj.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://umk.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://scc.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bpm.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fhs.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://erx.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zyd.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dji.xziqi.cn

[D26] 数组转字符串
来源：http://tvu.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://jlo.meibo888.top

PHP:  implode(", ", $arr);
来源：http://hpy.ydjk.org.cn

JS:   arr.join(", ")
来源：http://rxr.zhengqikj.top

TS:   arr.join(", ")
来源：http://qmo.aizwys.cn

Java: String.join(", ", list)
来源：http://ivx.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://anb.gogol.net.cn

Ruby: arr.join(", ")
来源：http://dkv.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://eay.c1oappe.top

================================================================================
来源：http://brd.nwbrower.top

E. 字符串处理
来源：http://lhg.smart0.xyz

================================================================================
来源：http://mep.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://fcb.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bhm.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mmb.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bgf.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ocd.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jla.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://erc.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bds.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfm.mhx1999.top

[E02] 重复字符串
来源：http://gki.tanke756.top

Py:   "ab" * 3
来源：http://asc.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://gbl.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://jbl.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://xez.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://shf.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://kww.yj202588.top

Ruby: "ab" * 3
来源：http://mep.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nzt.hammf.cn

[E03] 截取子串
来源：http://jak.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sty.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fnn.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqu.daria6918.cn

TS:   s.slice(1, 4)
来源：http://lhg.bjfxy.top

Java: s.substring(1, 4)
来源：http://viu.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gal.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://lvm.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://sjf.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://gmf.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://uqj.uphjek.com

PHP:  strpos($s, "x");
来源：http://alw.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nmd.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://sla.sysykeji.top

Java: s.indexOf("x")
来源：http://cny.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://sgg.vehdjk.com

Ruby: s.index("x")
来源：http://tum.yvedp.cn

C#:   s.IndexOf("x")
来源：http://mdb.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://tuf.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wjy.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yct.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mgk.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bgq.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdk.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xqn.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lad.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ycr.wangdashe.top

[E06] 替换子串
来源：http://tsw.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wbc.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://sdc.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ofm.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://fer.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jbh.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dzr.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jqz.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://sso.fehbvm.com

[E07] 按分隔符拆分
来源：http://juq.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qam.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yfu.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://thv.guowangkeji.top

TS:   s.split(",")
来源：http://fdy.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://mfy.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://alh.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://bmb.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rcu.zycfv.cn

[E08] 数组按分隔符合并
来源：http://bsj.jianghu66.top

Py:   ",".join(items)
来源：http://mgd.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://fqh.zhongyouzk.top

JS:   items.join(",")
来源：http://fey.pengpengdd.cyou

TS:   items.join(",")
来源：http://kjg.jlsjyb.cn

Java: String.join(",", items)
来源：http://nig.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://bvo.c1oappe.top

Ruby: items.join(",")
来源：http://dbx.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://iro.andypj.xyz

[E09] 去除所有空白字符
来源：http://rmt.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pha.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jja.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://gbd.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://bxh.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://hqn.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qob.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://wyy.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vgk.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://iyg.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgs.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://klp.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://ido.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://vjy.bjfxy.top

Java: String.format("%03d", 7)
来源：http://vyp.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://hjf.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pgq.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://msz.xinyue.icu

[E11] 反转字符串
来源：http://aja.gogol.net.cn

Py:   s[::-1]
来源：http://ayb.jlsjyb.cn

PHP:  strrev($s);
来源：http://vpy.meibo888.top

JS:   [...s].reverse().join("")
来源：http://hyc.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://aek.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kxt.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jbf.pengpengdd.cyou

Ruby: s.reverse
来源：http://htl.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eks.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://jgm.hfpthk.cn

Py:   s.count("a")
来源：http://hvb.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://bop.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://hxb.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://yyr.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azo.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://ruu.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://hcb.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://mxs.hesvh.cn

[E13] 逐字符遍历
来源：http://tac.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://dlz.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dyh.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://sem.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gmo.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://glj.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oas.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ekf.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kix.yueranfly.top

[E14] URL 编码与 Base64
来源：http://yfs.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uym.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ydf.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qjm.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xjb.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://emb.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://thp.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fub.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bti.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://yis.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://orh.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://inf.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zly.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bwu.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zoh.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkf.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://okv.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dls.haohaochexian.top

[E16] 数字千分位
来源：http://vmi.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://vfu.gogol.net.cn

PHP:  number_format(1234567);
来源：http://ibm.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://emf.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ftb.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://htx.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uwh.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vsk.cheryme.top

C#:   1234567.ToString("N0")
来源：http://now.jiagoushi.top

[E17] 首字母大写
来源：http://wiy.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://puo.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eol.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wuf.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yai.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hcg.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iww.gotoacloud.top

Ruby: s.capitalize
来源：http://qwq.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ukt.hammf.cn

[E18] 模板占位符替换
来源：http://xrp.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wpd.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wor.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bpo.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xre.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aba.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ytq.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hbl.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lht.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ekd.snrcjt.cn

Py:   s.splitlines()
来源：http://lzs.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vlg.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://znh.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://lfp.tarul.cn

Java: s.lines().toList()
来源：http://afq.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://bdi.ctjpmb.com

Ruby: s.lines
来源：http://zlr.tian-w.cn

C#:   s.Split('\n')
来源：http://kcb.yj20258.top

[E20] 判断字符串是否为空
来源：http://fpu.haohaochexian.top

Py:   if not s:
来源：http://qbu.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ije.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ljl.shuidangran.top

TS:   if (s === "") {}
来源：http://mvi.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://fsg.zdbjq.cn

Go:   if s == "" {}
来源：http://ccz.zhiwuduotai.top

Ruby: if s.empty?
来源：http://nvm.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fhz.zhixingplan.top

[E21] 超长截断加省略号
来源：http://ima.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xou.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://icr.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhg.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eqz.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kwx.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://ibv.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gnd.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cjb.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://qai.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mnr.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsk.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uxh.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipy.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://icu.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ucx.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://uvs.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qhq.9152youxi.cn

================================================================================
来源：http://wub.nwbrower.top

F. 文件与目录
来源：http://pvh.xingfuxueyuan.xyz

================================================================================
来源：http://szt.sxryk.cn

[F01] 读取整个文件
来源：http://oiq.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xdc.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://rmb.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gfw.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ias.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://owk.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xkp.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://esz.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://rmy.hnxiangtu.top

[F02] 逐行读取文件
来源：http://evs.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fwx.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nei.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyg.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uav.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gsq.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mpg.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jto.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://htx.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://xfh.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hce.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yrd.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlx.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rzs.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fbk.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jda.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://opj.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qpv.chenlongwang.top

[F04] 追加写入文件
来源：http://zmt.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jtw.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ltm.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqf.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kgf.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://toa.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mds.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://owd.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wsf.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://dek.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ebn.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://swp.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://fez.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://crt.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jjl.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zup.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://vwl.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://dnd.zhengqikj.top

[F06] 删除文件
来源：http://kin.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://gji.sxryk.cn

PHP:  unlink("a.txt");
来源：http://rto.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://gdh.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fnl.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dms.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://qzr.pycfn.com

Ruby: File.delete("a.txt")
来源：http://hxj.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://ebj.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://lok.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qvb.dianchejie.cn


<!-- 参考信息 -->