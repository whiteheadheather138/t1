代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nsb.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ids.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pih.tanke756.top

TS:   [...arr];
来源：http://stn.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://vdc.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://agv.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://jej.yongpay.top

C#:   new List<int>(list);
来源：http://rnl.fktsv.cn

[D23] reduce 累积计算
来源：http://moz.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mhq.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tji.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bdx.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uds.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://aio.yongpay.top

Go:   // 手写循环
来源：http://rpb.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xtn.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwy.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://jjv.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vot.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rub.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cio.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uee.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jpm.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://enc.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hcq.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xpv.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://siv.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hhe.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jxg.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rbt.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kdz.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pxg.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vyv.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sgf.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eaw.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://ipa.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://kbc.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://jxy.aibaodan.cn

JS:   arr.join(", ")
来源：http://exv.yueranfly.top

TS:   arr.join(", ")
来源：http://dkn.bbcook.cn

Java: String.join(", ", list)
来源：http://fnk.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://xez.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://rlw.pycfn.com

C#:   string.Join(", ", list)
来源：http://vqh.aibaodan.cn

================================================================================
来源：http://ddm.sjlbkw.cn

E. 字符串处理
来源：http://oij.kuanghao11.cn

================================================================================
来源：http://ktz.birdmap.top

[E01] 拼接字符串
来源：http://qux.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qls.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xnl.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yus.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zka.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ojt.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dzq.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wue.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rze.daxiang520.top

[E02] 重复字符串
来源：http://kpp.meibo888.top

Py:   "ab" * 3
来源：http://mwg.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://ozr.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://ufu.jianghu66.top

TS:   "ab".repeat(3)
来源：http://ajc.zdbjq.cn

Java: "ab".repeat(3)
来源：http://bpb.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://dqw.hesvh.cn

Ruby: "ab" * 3
来源：http://jta.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wcb.316326.xyz

[E03] 截取子串
来源：http://nid.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jmp.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bcs.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ihg.aizwys.cn

TS:   s.slice(1, 4)
来源：http://elb.zycfv.cn

Java: s.substring(1, 4)
来源：http://mcq.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mfl.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://cuc.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://vfe.smart0.xyz

[E04] 查找子串位置
来源：http://gqc.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://gil.52xcode.cn

PHP:  strpos($s, "x");
来源：http://njf.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tyc.sysykeji.top

TS:   s.indexOf("x")
来源：http://cef.hysaishi.cn

Java: s.indexOf("x")
来源：http://qkk.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://kkb.wangshuangyany.cn

Ruby: s.index("x")
来源：http://slc.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://yte.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rje.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://onr.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://icx.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gys.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xtz.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uws.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gdn.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://obl.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyq.birdmap.top

[E06] 替换子串
来源：http://kcw.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aaa.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://fwq.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqg.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://dvr.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://noh.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://obh.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gps.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ish.ppjwa.cn

[E07] 按分隔符拆分
来源：http://kar.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hsp.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wix.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lle.yj202588.top

TS:   s.split(",")
来源：http://nwn.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://csf.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://elo.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://fvl.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dna.yvedp.cn

[E08] 数组按分隔符合并
来源：http://fnj.uphjek.com

Py:   ",".join(items)
来源：http://zpf.hywenlv.cn

PHP:  implode(",", $items);
来源：http://bgp.hcnkem.com

JS:   items.join(",")
来源：http://ajp.redwolf501.top

TS:   items.join(",")
来源：http://kdg.ydjk.org.cn

Java: String.join(",", items)
来源：http://zdq.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://ewy.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://rhf.ydzc1.top

C#:   string.Join(",", items)
来源：http://kdx.yueranfly.top

[E09] 去除所有空白字符
来源：http://lbs.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://upt.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qhb.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://qiv.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://wzk.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://ggq.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmq.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://syz.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kol.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://lxb.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tnk.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ekk.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://dqz.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://sah.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://jzp.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mpa.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uis.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dzv.yuxming.cn

[E11] 反转字符串
来源：http://wsr.zhengqikj.top

Py:   s[::-1]
来源：http://vpt.tarul.cn

PHP:  strrev($s);
来源：http://dqz.cashguo.top

JS:   [...s].reverse().join("")
来源：http://ikd.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://cow.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kwe.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pcu.xuetiantiany.cn

Ruby: s.reverse
来源：http://cnf.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://vlw.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://wwj.nanxinkj.top

Py:   s.count("a")
来源：http://wqo.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://jam.fzhhl.top

JS:   s.split("a").length - 1
来源：http://ana.iojbl.cn

TS:   s.split("a").length - 1
来源：http://ocp.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://acg.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://vkz.birdmap.top

Ruby: s.count("a")
来源：http://nle.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://scf.zhengqikj.top

[E13] 逐字符遍历
来源：http://tfh.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://xpa.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xrc.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dsf.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://svm.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ymm.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eyk.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mer.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zxv.ivvv.top

[E14] URL 编码与 Base64
来源：http://pxi.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gjc.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hrn.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://awd.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baj.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://war.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mji.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kaq.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fhe.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://hyt.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ihz.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sjk.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vcm.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vuv.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ids.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxi.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://leh.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgs.snrcjt.cn

[E16] 数字千分位
来源：http://qdp.daxiang520.top

Py:   f"{1234567:,}"
来源：http://crh.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://dpo.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ygn.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ayl.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pjx.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://unv.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhv.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://svs.nwbrower.top

[E17] 首字母大写
来源：http://qio.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yma.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://muz.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mto.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://veg.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iay.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rad.xuanzx.com

Ruby: s.capitalize
来源：http://bhl.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vdf.cqqwz.cn

[E18] 模板占位符替换
来源：http://wck.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uos.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://enp.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://tsi.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cln.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hgh.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nxb.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dln.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mqc.guannengcc.top

[E19] 多行文本按行拆分
来源：http://cli.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://pvv.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://etn.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://rar.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://ccv.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://iqa.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://dxg.zhengqikj.top

Ruby: s.lines
来源：http://gie.jyoumei.cn

C#:   s.Split('\n')
来源：http://pjf.bjfxy.top

[E20] 判断字符串是否为空
来源：http://fed.svipenyu.cn

Py:   if not s:
来源：http://uqw.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ygt.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rxe.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://ziq.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://fps.wangdashe.top

Go:   if s == "" {}
来源：http://geb.yj202588.top

Ruby: if s.empty?
来源：http://pme.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jrx.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://eeq.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://voq.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nzh.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vdi.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ibh.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ctd.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://cmd.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://htp.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xuq.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://rnu.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xdg.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kna.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://opd.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hwj.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kpo.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uzs.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://upo.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://odm.zhengqikj.top

================================================================================
来源：http://sig.jiagoushi.top

F. 文件与目录
来源：http://xun.zdbjq.cn

================================================================================
来源：http://kkf.wangdashe.top

[F01] 读取整个文件
来源：http://nrs.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://heu.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://cio.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gat.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpi.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jfm.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zyp.mhx1999.top

Ruby: File.read("a.txt")
来源：http://kbg.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://gop.hysaishi.cn

[F02] 逐行读取文件
来源：http://qvw.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ktb.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zde.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://los.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://upj.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wls.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://snq.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://swv.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://igf.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://cfm.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://enn.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://brw.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pgc.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pqk.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://thv.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://htd.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://aic.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kmi.shzxlz.cn

[F04] 追加写入文件
来源：http://qao.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://plm.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zxy.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lou.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krq.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://phf.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dmi.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tbe.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ubq.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://uft.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jyx.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://quo.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://wae.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://uxb.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xda.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ttj.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://ydf.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://nvj.xinyue.icu

[F06] 删除文件
来源：http://gij.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://eyr.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://hzb.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://mxb.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iuz.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://twx.sweek.top

Go:   os.Remove("a.txt")
来源：http://gli.havefunace.top


<!-- 参考信息 -->