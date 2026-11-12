代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xkr.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wuo.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rtp.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://hpy.bbcook.cn

Ruby: arr.tally
来源：http://wuh.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hto.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://lfd.yj20258.top

Py:   x in arr
来源：http://nsf.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://pxk.yuxming.cn

JS:   arr.includes(x)
来源：http://bxc.chenzaomai.com

TS:   arr.includes(x)
来源：http://xbd.nanxuanxn.top

Java: list.contains(x)
来源：http://emh.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://epe.haohaochexian.top

Ruby: arr.include?(x)
来源：http://som.yvedp.cn

C#:   list.Contains(x)
来源：http://kpd.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://ayb.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://brc.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dsw.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gdh.epnwcf.com

TS:   [...arr];
来源：http://tno.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://jqg.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://cli.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://job.xylfe.cn

C#:   new List<int>(list);
来源：http://ugh.bbcook.cn

[D23] reduce 累积计算
来源：http://onj.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tel.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rve.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvy.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rrk.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rbh.yuanzhike.top

Go:   // 手写循环
来源：http://obc.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xwi.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dha.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://ubc.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xdq.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qqp.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sxt.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aim.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fre.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vmz.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jkp.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tki.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://onx.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mxr.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ckg.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yrx.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggn.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ouw.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baz.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ylb.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vaf.tianlin.xyz

[D26] 数组转字符串
来源：http://kmc.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://mvo.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://pjy.0kj1m.cn

JS:   arr.join(", ")
来源：http://jnr.hysaishi.cn

TS:   arr.join(", ")
来源：http://siv.nanxuanxn.top

Java: String.join(", ", list)
来源：http://sth.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://hyw.52xcode.cn

Ruby: arr.join(", ")
来源：http://gne.bbcook.cn

C#:   string.Join(", ", list)
来源：http://dzv.yj20258.top

================================================================================
来源：http://rqc.mhx1999.top

E. 字符串处理
来源：http://zrl.zhoulong.xyz

================================================================================
来源：http://gpr.bjfxy.top

[E01] 拼接字符串
来源：http://tkc.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ysc.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qha.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lof.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lin.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qzi.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nuc.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pkm.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://alv.nanxuanxn.top

[E02] 重复字符串
来源：http://dxr.daria6918.cn

Py:   "ab" * 3
来源：http://cdk.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://byt.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://ovn.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://esk.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://tef.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://yif.gotoacloud.top

Ruby: "ab" * 3
来源：http://cva.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aaf.chenlongwang.top

[E03] 截取子串
来源：http://vlf.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gte.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://trw.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://plg.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://ero.zhixingplan.top

Java: s.substring(1, 4)
来源：http://zdb.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gqu.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://upz.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://rql.chenzaomai.com

[E04] 查找子串位置
来源：http://img.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://ixv.ybcxt.top

PHP:  strpos($s, "x");
来源：http://ida.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://prx.jyoumei.cn

TS:   s.indexOf("x")
来源：http://ubf.smart0.xyz

Java: s.indexOf("x")
来源：http://hzm.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://afk.guowangkeji.top

Ruby: s.index("x")
来源：http://ege.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://kzp.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aov.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqt.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jdp.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vem.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lme.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fya.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jey.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iic.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dbs.guannengcc.top

[E06] 替换子串
来源：http://etk.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uez.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://kgg.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sal.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://tpn.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://azp.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oew.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ncl.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://wpn.sysykeji.top

[E07] 按分隔符拆分
来源：http://ccn.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://swh.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qfo.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://rud.xuetiantiany.cn

TS:   s.split(",")
来源：http://kye.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://adj.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bhh.sweek.top

Ruby: s.split(",");  s.split
来源：http://cdt.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://slt.hnqzz.top

[E08] 数组按分隔符合并
来源：http://ofm.jqgufenzy.top

Py:   ",".join(items)
来源：http://ecs.snrcjt.cn

PHP:  implode(",", $items);
来源：http://eod.yj20258888.top

JS:   items.join(",")
来源：http://nsy.gaohongyu789.top

TS:   items.join(",")
来源：http://azv.feifeiyinyue.top

Java: String.join(",", items)
来源：http://wqv.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://gri.dashuyun.cn

Ruby: items.join(",")
来源：http://iwj.hywenlv.cn

C#:   string.Join(",", items)
来源：http://yvy.cdnleiting.top

[E09] 去除所有空白字符
来源：http://deh.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hoh.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aud.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://jpw.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://bad.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://fol.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fpg.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://fzq.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wtj.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://rts.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mnf.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tct.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://lgi.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://zkv.wangdashe.top

Java: String.format("%03d", 7)
来源：http://alg.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hnx.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cln.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bjj.cqqwz.cn

[E11] 反转字符串
来源：http://ygw.gogol.net.cn

Py:   s[::-1]
来源：http://fen.guowangkeji.top

PHP:  strrev($s);
来源：http://tuq.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://hop.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://kgk.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ail.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gyr.chenzaomai.com

Ruby: s.reverse
来源：http://nal.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://izt.yuxming.cn

[E12] 统计某字符出现次数
来源：http://rif.yvedp.cn

Py:   s.count("a")
来源：http://xln.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://vyz.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://rhb.ydzc1.top

TS:   s.split("a").length - 1
来源：http://hkn.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qbx.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://iia.0kj1m.cn

Ruby: s.count("a")
来源：http://vjh.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://dma.bjfxy.top

[E13] 逐字符遍历
来源：http://wqq.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://rus.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://msh.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gsu.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hbg.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fhh.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cem.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://spm.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wcg.havefunace.top

[E14] URL 编码与 Base64
来源：http://chm.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blf.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ato.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nmb.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pmd.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mqh.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kgp.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ogo.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ljq.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://zud.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://vpo.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uge.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pvc.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://cnn.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uxt.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ezn.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cxp.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fya.zhijiandao.cn

[E16] 数字千分位
来源：http://pib.xinyue.icu

Py:   f"{1234567:,}"
来源：http://tuf.yuxming.cn

PHP:  number_format(1234567);
来源：http://eaw.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vks.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pnd.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxo.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://smp.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwf.uphjek.com

C#:   1234567.ToString("N0")
来源：http://ogk.birdmap.top

[E17] 首字母大写
来源：http://ofz.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fav.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://cuw.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nfu.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kje.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gbu.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://csv.bbcook.cn

Ruby: s.capitalize
来源：http://kgn.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rbp.ctjpmb.com

[E18] 模板占位符替换
来源：http://ifh.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eai.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fyz.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bfx.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://fps.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pjv.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nre.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://esq.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fbs.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://yms.ehwqpu.com

Py:   s.splitlines()
来源：http://ncr.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hmu.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://nxn.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://mep.cucudq.cn

Java: s.lines().toList()
来源：http://bcm.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://ikh.aizwys.cn

Ruby: s.lines
来源：http://zav.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://ylf.sweek.top

[E20] 判断字符串是否为空
来源：http://ydr.pycfn.com

Py:   if not s:
来源：http://itt.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vrb.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://msn.bjfxy.top

TS:   if (s === "") {}
来源：http://orm.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://zug.bjfxy.top

Go:   if s == "" {}
来源：http://wut.xinyue.icu

Ruby: if s.empty?
来源：http://dgt.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ivc.ydzc1.top

[E21] 超长截断加省略号
来源：http://iof.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yix.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xid.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vak.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pti.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bll.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://iko.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cvg.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bku.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://buf.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xfj.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://idu.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://brc.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvf.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mfp.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nkg.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://xaz.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://icw.yangfankeji.com

================================================================================
来源：http://kbh.fktsv.cn

F. 文件与目录
来源：http://fsx.yj20258.top

================================================================================
来源：http://vrk.yangfankeji.com

[F01] 读取整个文件
来源：http://fai.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://avj.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://ecp.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sfg.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jja.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ipg.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rhe.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://ujy.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://sak.andypj.xyz

[F02] 逐行读取文件
来源：http://ewi.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ayb.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wxe.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vlz.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tgk.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lpv.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://njy.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zyv.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ebf.uphjek.com

[F03] 写入文件（覆盖）
来源：http://dkm.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aiu.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jcm.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://knz.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://edp.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tjp.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kwi.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://chn.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zuh.aizwys.cn

[F04] 追加写入文件
来源：http://lik.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ngc.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hhl.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pfi.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfw.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lva.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ksr.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xsm.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nrq.xziqi.cn


<!-- 参考信息 -->