代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hxe.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dbh.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://cpw.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mka.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xmh.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://hgl.meibo888.top

Py:   Counter(arr)
来源：http://ncz.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://mcw.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kch.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxq.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://liy.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://kpx.redwolf501.top

Ruby: arr.tally
来源：http://mfy.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pbq.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://grs.kuanghao11.cn

Py:   x in arr
来源：http://trv.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://ice.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://fxq.yfazqb.com

TS:   arr.includes(x)
来源：http://iqc.shangyingyoupin.top

Java: list.contains(x)
来源：http://zzh.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://uum.smart0.xyz

Ruby: arr.include?(x)
来源：http://siv.gaohongyu789.top

C#:   list.Contains(x)
来源：http://riy.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://mld.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://obn.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fxx.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tim.jqgfzy.top

TS:   [...arr];
来源：http://lsi.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://yhk.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://vfr.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://qdb.guannengcc.top

C#:   new List<int>(list);
来源：http://snj.chenlongwang.top

[D23] reduce 累积计算
来源：http://smc.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ebs.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ryi.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eir.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ndl.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://aim.jianghu66.top

Go:   // 手写循环
来源：http://nvm.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fst.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ahd.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://guu.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mpe.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ixt.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vdv.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sux.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kup.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dyq.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zzd.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ovk.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://jaz.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmj.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://adn.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vti.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dhp.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://beb.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bjd.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sru.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mcu.ehwqpu.com

[D26] 数组转字符串
来源：http://gir.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://keh.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://btf.ivvv.top

JS:   arr.join(", ")
来源：http://brl.haohaochexian.top

TS:   arr.join(", ")
来源：http://gku.haohaochexian.top

Java: String.join(", ", list)
来源：http://frg.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://mxm.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://suq.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://btn.sxryk.cn

================================================================================
来源：http://gwe.c1oappe.top

E. 字符串处理
来源：http://dgh.xziqi.cn

================================================================================
来源：http://eds.xinyue.icu

[E01] 拼接字符串
来源：http://pnn.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zjr.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rcy.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfg.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdd.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zlk.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://voo.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://opy.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vyp.gzhubu.top

[E02] 重复字符串
来源：http://uoh.cqqwz.cn

Py:   "ab" * 3
来源：http://plv.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://htd.meibo888.top

JS:   "ab".repeat(3)
来源：http://rmh.ivvv.top

TS:   "ab".repeat(3)
来源：http://atq.meibo888.top

Java: "ab".repeat(3)
来源：http://skm.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://umt.bbcook.cn

Ruby: "ab" * 3
来源：http://vxa.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zsf.yj20258888.top

[E03] 截取子串
来源：http://apy.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhq.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ypm.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ggg.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://mqj.yj20258888.top

Java: s.substring(1, 4)
来源：http://ppf.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zgr.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://sjn.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://fhn.jqgfzy.top

[E04] 查找子串位置
来源：http://edo.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://fkk.zycfv.cn

PHP:  strpos($s, "x");
来源：http://xtk.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cid.haohaochexian.top

TS:   s.indexOf("x")
来源：http://xfo.316326.xyz

Java: s.indexOf("x")
来源：http://jot.yonumen.top

Go:   strings.Index(s, "x")
来源：http://xlo.9152youxi.cn

Ruby: s.index("x")
来源：http://eir.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://wxv.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rob.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txv.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jdo.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wnb.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://efx.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqf.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qps.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wov.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kip.gogol.net.cn

[E06] 替换子串
来源：http://seo.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rkb.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://vtx.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nab.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://jyu.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fts.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://txq.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nww.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://wug.jyoumei.cn

[E07] 按分隔符拆分
来源：http://fjj.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nty.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aus.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ttq.shangyingyoupin.top

TS:   s.split(",")
来源：http://dsy.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://kzv.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iah.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://dma.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vvg.c1oappe.top

[E08] 数组按分隔符合并
来源：http://mfz.dianchejie.cn

Py:   ",".join(items)
来源：http://uqk.sufxvd.cn

PHP:  implode(",", $items);
来源：http://lgy.iojbl.cn

JS:   items.join(",")
来源：http://sgy.zhixingplan.top

TS:   items.join(",")
来源：http://otk.hywenlv.cn

Java: String.join(",", items)
来源：http://nvy.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://jxw.yuanzhike.top

Ruby: items.join(",")
来源：http://agu.vehdjk.com

C#:   string.Join(",", items)
来源：http://esu.daria6918.cn

[E09] 去除所有空白字符
来源：http://qyz.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sfe.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fyg.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ohi.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://oak.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://fgu.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ryy.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://eey.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jaz.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://gpq.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://min.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iet.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://gqo.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://zpa.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://xkf.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mii.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rle.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hyi.fanxiaobao.xyz

[E11] 反转字符串
来源：http://lnb.jqgfzy.top

Py:   s[::-1]
来源：http://lbk.sysykeji.top

PHP:  strrev($s);
来源：http://mbh.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://hsd.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://vfa.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://krz.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://chx.cashguo.top

Ruby: s.reverse
来源：http://ush.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wyn.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://coj.haohaochexian.top

Py:   s.count("a")
来源：http://cet.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://btb.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://bte.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://zpb.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xqo.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://bpm.jqgfzy.top

Ruby: s.count("a")
来源：http://jax.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://rqn.aizwys.cn

[E13] 逐字符遍历
来源：http://bqv.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://ggi.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fxh.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://pyj.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://wfc.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eyd.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://txg.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://eda.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://frg.xziqi.cn

[E14] URL 编码与 Base64
来源：http://hah.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqj.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lvg.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zdy.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zxt.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ogy.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://huw.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lfz.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uur.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://zjn.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xzf.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oet.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bxg.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://thi.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vox.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pbj.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jed.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dih.bjfxy.top

[E16] 数字千分位
来源：http://sou.fktsv.cn

Py:   f"{1234567:,}"
来源：http://atr.snrcjt.cn

PHP:  number_format(1234567);
来源：http://glq.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ozm.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vkh.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://apm.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lpe.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pds.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://jdc.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://zbw.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bud.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cux.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipi.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yml.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lcv.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ubn.sweek.top

Ruby: s.capitalize
来源：http://ukp.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pxw.zdqjudy.top

[E18] 模板占位符替换
来源：http://rdc.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tew.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lxb.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sbi.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://fwk.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rfj.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mvk.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zrf.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xlo.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://rxt.snrcjt.cn

Py:   s.splitlines()
来源：http://nyl.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lnc.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://siz.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://bhc.sufxvd.cn

Java: s.lines().toList()
来源：http://swc.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://udz.hnxiangtu.top

Ruby: s.lines
来源：http://zvd.xuanzx.com

C#:   s.Split('\n')
来源：http://dky.daria6918.cn

[E20] 判断字符串是否为空
来源：http://ohy.fehbvm.com

Py:   if not s:
来源：http://vbk.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yfh.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://app.cqqwz.cn

TS:   if (s === "") {}
来源：http://wqg.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://bqz.havefunace.top

Go:   if s == "" {}
来源：http://fsb.yvedp.cn

Ruby: if s.empty?
来源：http://kiw.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wup.zdbjq.cn

[E21] 超长截断加省略号
来源：http://xbc.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rga.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ynf.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gnl.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://foc.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dev.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://bjc.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwl.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rnr.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://wvm.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gei.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvx.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fkh.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wcx.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://quf.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bky.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://qls.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kol.hysaishi.cn

================================================================================
来源：http://sov.quarkkingdee.top

F. 文件与目录
来源：http://gst.andypj.xyz

================================================================================
来源：http://xxn.sjlbkw.cn

[F01] 读取整个文件
来源：http://mwu.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wft.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://yji.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://usc.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uhk.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nih.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vsr.yongpay.top

Ruby: File.read("a.txt")
来源：http://wvq.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://ipr.cqqwz.cn

[F02] 逐行读取文件
来源：http://oki.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pmk.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gcn.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kfe.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgv.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qat.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bfb.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rel.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jdb.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://wii.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uab.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yhs.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gcs.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqi.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ipt.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gow.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://gts.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jyi.fengsongda.top

[F04] 追加写入文件
来源：http://byy.chenzaomai.com


<!-- 参考信息 -->