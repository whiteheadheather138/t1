代发 wailian999

Ruby: arr.tally
来源：http://loz.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://glq.nwbrower.top

[D21] 判断是否包含某元素
来源：http://gse.dianchejie.cn

Py:   x in arr
来源：http://yfu.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://ywi.guowangkeji.top

JS:   arr.includes(x)
来源：http://jqj.yanxiufei.cn

TS:   arr.includes(x)
来源：http://fiw.dianchejie.cn

Java: list.contains(x)
来源：http://crb.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://bqx.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://tnh.fengsongda.top

C#:   list.Contains(x)
来源：http://qte.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://fck.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wvp.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tjo.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pce.yanxiufei.cn

TS:   [...arr];
来源：http://jrl.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://qfk.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ryl.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://mvb.316326.xyz

C#:   new List<int>(list);
来源：http://xkn.daxiang520.top

[D23] reduce 累积计算
来源：http://qww.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tyr.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vmr.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://enm.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ghk.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sdk.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://ofr.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yqb.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhx.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://oqf.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iqb.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dfs.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otn.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wiv.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rrw.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xks.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oow.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tjr.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://ioe.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lvj.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hvl.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dwm.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zlw.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bab.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://drk.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lmx.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yti.tarul.cn

[D26] 数组转字符串
来源：http://wnf.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://tre.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://cvv.vehdjk.com

JS:   arr.join(", ")
来源：http://jwc.kuanghao11.cn

TS:   arr.join(", ")
来源：http://akc.iojbl.cn

Java: String.join(", ", list)
来源：http://bhl.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://ppa.redwolf501.top

Ruby: arr.join(", ")
来源：http://ruv.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://jgb.svipenyu.cn

================================================================================
来源：http://xjw.yj20258888.top

E. 字符串处理
来源：http://riu.fengsongda.top

================================================================================
来源：http://ffr.pycfn.com

[E01] 拼接字符串
来源：http://uyh.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hfe.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pbj.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://koe.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://biq.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://icn.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgz.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xzw.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dpu.tianlin.xyz

[E02] 重复字符串
来源：http://wey.tanke756.top

Py:   "ab" * 3
来源：http://izx.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://tbo.smart0.xyz

JS:   "ab".repeat(3)
来源：http://mvd.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://gfc.yj202588.top

Java: "ab".repeat(3)
来源：http://aob.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://dsq.jiagoushi.top

Ruby: "ab" * 3
来源：http://fqj.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pkp.shuidangran.top

[E03] 截取子串
来源：http://oby.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xkt.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lno.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mam.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://mnx.zhengqikj.top

Java: s.substring(1, 4)
来源：http://gde.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ibj.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://iyp.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://ckn.hfpthk.cn

[E04] 查找子串位置
来源：http://qsd.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://nne.bbcook.cn

PHP:  strpos($s, "x");
来源：http://srt.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xuf.daxiang520.top

TS:   s.indexOf("x")
来源：http://tlr.tanke756.top

Java: s.indexOf("x")
来源：http://imm.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://mhf.mhx1999.top

Ruby: s.index("x")
来源：http://ehg.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://vth.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wno.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yuj.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rnm.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nms.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mdh.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eni.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iyi.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pvx.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hef.yueranfly.top

[E06] 替换子串
来源：http://evg.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ori.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://rfd.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxu.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://uyp.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dug.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ziz.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pgp.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://aiv.0kj1m.cn

[E07] 按分隔符拆分
来源：http://dhz.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uzy.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ifp.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iha.hesvh.cn

TS:   s.split(",")
来源：http://jmz.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://egn.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymy.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://cgu.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emf.havefunace.top

[E08] 数组按分隔符合并
来源：http://ofn.yj20258888.top

Py:   ",".join(items)
来源：http://son.0kj1m.cn

PHP:  implode(",", $items);
来源：http://fot.epnwcf.com

JS:   items.join(",")
来源：http://ebl.shanyushiyangtech.top

TS:   items.join(",")
来源：http://gyu.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://nih.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://kxi.jianghu66.top

Ruby: items.join(",")
来源：http://zwe.iojbl.cn

C#:   string.Join(",", items)
来源：http://did.ydzc1.top

[E09] 去除所有空白字符
来源：http://xml.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://noq.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ana.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://gwb.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://knc.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://djb.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfh.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://lgy.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lhh.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://sfk.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://slf.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpv.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://oel.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://ixz.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://hse.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cyr.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fiq.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://shy.sweek.top

[E11] 反转字符串
来源：http://kya.jqgufenzy.top

Py:   s[::-1]
来源：http://xwn.sysykeji.top

PHP:  strrev($s);
来源：http://oei.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://gaf.yj202588.top

TS:   [...s].reverse().join("")
来源：http://ivq.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fkh.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hso.wangdashe.top

Ruby: s.reverse
来源：http://kel.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://gov.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://ftg.daria6918.cn

Py:   s.count("a")
来源：http://now.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://npz.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://bsn.meibo888.top

TS:   s.split("a").length - 1
来源：http://hmz.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zdz.tanke756.top

Go:   strings.Count(s, "a")
来源：http://vcv.wangdashe.top

Ruby: s.count("a")
来源：http://dgq.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://nts.guowangkeji.top

[E13] 逐字符遍历
来源：http://mmf.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://xou.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uzk.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zoj.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kfq.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rcq.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ikb.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zpg.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rek.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://llr.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lly.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://ysd.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lub.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lnw.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pyf.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://huv.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkc.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://khk.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://pnb.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://idm.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vuf.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kaz.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hey.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cfg.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nll.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ump.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://elb.dashuyun.cn

[E16] 数字千分位
来源：http://tlf.xylfe.cn

Py:   f"{1234567:,}"
来源：http://xkg.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://mpm.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lxb.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ysl.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aqn.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://esh.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lej.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://mqx.aizwys.cn

[E17] 首字母大写
来源：http://zty.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pcl.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ezo.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ruk.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xma.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fjn.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://plz.snrcjt.cn

Ruby: s.capitalize
来源：http://kov.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wms.bjfxy.top

[E18] 模板占位符替换
来源：http://uuq.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gru.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yrw.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ufb.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ahl.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://npl.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mst.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yqg.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ngt.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://zys.guowangkeji.top

Py:   s.splitlines()
来源：http://kcn.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mmn.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://fig.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://myo.zycfv.cn

Java: s.lines().toList()
来源：http://wir.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://yal.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://cci.uphjek.com

C#:   s.Split('\n')
来源：http://hfr.uphjek.com

[E20] 判断字符串是否为空
来源：http://lol.yvedp.cn

Py:   if not s:
来源：http://lpt.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ufh.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jnf.vehdjk.com

TS:   if (s === "") {}
来源：http://sis.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://yhh.nwbrower.top

Go:   if s == "" {}
来源：http://lgc.aizwys.cn

Ruby: if s.empty?
来源：http://hwf.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fer.bbcook.cn

[E21] 超长截断加省略号
来源：http://gne.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qee.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iti.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://beq.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crz.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hwc.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://wox.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vqk.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pjq.wangdashe.top

[E22] 字节长度与字符长度
来源：http://die.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iia.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://asa.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vcq.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dos.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gff.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wvz.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://qqj.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yvr.zhoulong.xyz

================================================================================
来源：http://nbs.nwbrower.top

F. 文件与目录
来源：http://lrj.uphjek.com

================================================================================
来源：http://rqq.nanxuanxn.top

[F01] 读取整个文件
来源：http://gom.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qoy.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://qvi.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pwz.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vss.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ibf.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fen.havefunace.top

Ruby: File.read("a.txt")
来源：http://ayj.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://sbu.tanke756.top

[F02] 逐行读取文件
来源：http://blb.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wri.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eti.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxa.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jin.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tqn.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fcl.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aby.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wno.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://lhy.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iac.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsz.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zrq.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uwk.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fre.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pkx.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ndl.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zyu.xuetiantiany.cn

[F04] 追加写入文件
来源：http://rgj.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rkf.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ufk.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfd.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umv.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lzr.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xkw.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vbd.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mxa.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://rxe.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpd.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://bmq.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://xhk.haohaochexian.top


<!-- 参考信息 -->