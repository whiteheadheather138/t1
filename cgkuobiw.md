代发 wailian999

Ruby: arr.tally
来源：http://juz.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ura.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://gdk.ivvv.top

Py:   x in arr
来源：http://vpy.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://ign.yvedp.cn

JS:   arr.includes(x)
来源：http://elm.yvedp.cn

TS:   arr.includes(x)
来源：http://ogy.zhijiandao.cn

Java: list.contains(x)
来源：http://ihr.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://qfj.sysykeji.top

Ruby: arr.include?(x)
来源：http://qqf.redwolf501.top

C#:   list.Contains(x)
来源：http://out.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://gwc.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://stq.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://exy.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://odq.hesvh.cn

TS:   [...arr];
来源：http://inf.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://kaw.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://bku.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://kjm.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://ugm.uphjek.com

[D23] reduce 累积计算
来源：http://vun.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tgt.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fzq.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxd.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upr.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tcu.zhiwuduotai.top

Go:   // 手写循环
来源：http://anm.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fvq.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lxw.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://kqr.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vqn.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oim.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kpp.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vsr.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ubl.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zhw.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gnh.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dhk.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://bhr.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uwn.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gky.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yub.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tit.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dje.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uux.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uxr.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://omh.uphjek.com

[D26] 数组转字符串
来源：http://kbe.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://lxa.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://dwf.cheryme.top

JS:   arr.join(", ")
来源：http://cmd.aibaodan.cn

TS:   arr.join(", ")
来源：http://rog.yfazqb.com

Java: String.join(", ", list)
来源：http://pxt.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://exd.pycfn.com

Ruby: arr.join(", ")
来源：http://ifj.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://gmh.daria6918.cn

================================================================================
来源：http://end.ydjk.org.cn

E. 字符串处理
来源：http://gog.ybcxt.top

================================================================================
来源：http://ibq.shuidangran.top

[E01] 拼接字符串
来源：http://obj.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ccq.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hjy.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zuz.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tnf.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://enl.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lyn.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://peu.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzp.gzhubu.top

[E02] 重复字符串
来源：http://rtv.haohaochexian.top

Py:   "ab" * 3
来源：http://iwv.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://wgp.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://kzg.52xcode.cn

TS:   "ab".repeat(3)
来源：http://nel.gogol.net.cn

Java: "ab".repeat(3)
来源：http://dqu.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://fln.dianchejie.cn

Ruby: "ab" * 3
来源：http://jpn.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fsn.birdmap.top

[E03] 截取子串
来源：http://zpi.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jcs.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fqt.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ned.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://mpy.zdbjq.cn

Java: s.substring(1, 4)
来源：http://oeh.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ifx.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xna.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://pvl.ydjk.org.cn

[E04] 查找子串位置
来源：http://ltk.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://xfm.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://tyl.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pyt.svipenyu.cn

TS:   s.indexOf("x")
来源：http://muw.yuxming.cn

Java: s.indexOf("x")
来源：http://tmk.sweek.top

Go:   strings.Index(s, "x")
来源：http://xvi.jqgfzy.top

Ruby: s.index("x")
来源：http://lxo.xziqi.cn

C#:   s.IndexOf("x")
来源：http://xkw.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eas.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pfw.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hwp.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lau.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oob.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mlu.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jmm.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zjr.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sax.chenjidiqi.icu

[E06] 替换子串
来源：http://tnr.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aau.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://ywb.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ivn.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://xty.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pxg.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aef.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://plo.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://neh.svipenyu.cn

[E07] 按分隔符拆分
来源：http://yqt.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sbm.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zka.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dhr.shuidangran.top

TS:   s.split(",")
来源：http://hfe.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qbn.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qel.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://psg.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ywf.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://rwd.chenlongwang.top

Py:   ",".join(items)
来源：http://uvp.sxryk.cn

PHP:  implode(",", $items);
来源：http://vfv.xinyue.icu

JS:   items.join(",")
来源：http://ehp.9152youxi.cn

TS:   items.join(",")
来源：http://imu.cheryme.top

Java: String.join(",", items)
来源：http://kno.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://vcd.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://vyf.daria6918.cn

C#:   string.Join(",", items)
来源：http://duu.uphjek.com

[E09] 去除所有空白字符
来源：http://acj.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pop.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ugg.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://uym.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://uce.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://dcy.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dae.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://ojz.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hom.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://swm.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://evd.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vut.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://nby.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://mzh.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://jgs.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://atq.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://joe.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://acv.hcnkem.com

[E11] 反转字符串
来源：http://hkc.jqgufenzy.top

Py:   s[::-1]
来源：http://qgu.zhoulong.xyz

PHP:  strrev($s);
来源：http://dyq.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://pzd.cashguo.top

TS:   [...s].reverse().join("")
来源：http://eni.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wzv.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mvu.chenlongwang.top

Ruby: s.reverse
来源：http://luo.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://vgp.yueranfly.top

[E12] 统计某字符出现次数
来源：http://kiu.snrcjt.cn

Py:   s.count("a")
来源：http://kgn.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://odh.guannengcc.top

JS:   s.split("a").length - 1
来源：http://fva.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://wat.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vlv.birdmap.top

Go:   strings.Count(s, "a")
来源：http://trg.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://rsi.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://lry.smart0.xyz

[E13] 逐字符遍历
来源：http://rsr.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://mqv.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fce.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://xkk.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sus.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsq.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ump.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lni.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhg.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://pyt.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://caq.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hon.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afr.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dtw.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jlp.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://liv.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qse.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qlg.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://glp.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vgy.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bip.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bav.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vop.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ojj.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oqj.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rjr.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bib.yj20258888.top

[E16] 数字千分位
来源：http://lqu.hnqzz.top

Py:   f"{1234567:,}"
来源：http://ifp.yongpay.top

PHP:  number_format(1234567);
来源：http://yws.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://emf.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ejx.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vgn.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ndb.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uou.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://aiz.yanxiufei.cn

[E17] 首字母大写
来源：http://rvp.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nkl.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gzh.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rys.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tea.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hxd.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oku.sysykeji.top

Ruby: s.capitalize
来源：http://kmg.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hbh.fktsv.cn

[E18] 模板占位符替换
来源：http://via.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wbh.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfk.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lws.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uxl.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://feb.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fqu.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ecz.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lvp.hnqzz.top

[E19] 多行文本按行拆分
来源：http://rzh.zhongyouzk.top

Py:   s.splitlines()
来源：http://xmm.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ctl.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://rxe.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://ltn.birdmap.top

Java: s.lines().toList()
来源：http://qzc.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://nap.ydjk.org.cn

Ruby: s.lines
来源：http://gna.9152youxi.cn

C#:   s.Split('\n')
来源：http://fyp.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://ghb.ppjwa.cn

Py:   if not s:
来源：http://cao.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rec.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gyp.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://ccy.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://jvy.chenzaomai.com

Go:   if s == "" {}
来源：http://zta.shzxlz.cn

Ruby: if s.empty?
来源：http://qxc.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vyp.tarul.cn

[E21] 超长截断加省略号
来源：http://hgq.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aeq.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezw.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jmv.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbf.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tpj.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://zox.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kvm.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jeu.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://tbo.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kgc.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://frw.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://duk.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sbo.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqi.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hso.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://usm.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ijb.zycfv.cn

================================================================================
来源：http://esi.dashuyun.cn

F. 文件与目录
来源：http://sjj.chenjidiqi.icu

================================================================================
来源：http://jlv.cqqwz.cn

[F01] 读取整个文件
来源：http://icd.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jmg.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://usu.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dgk.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gok.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gks.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ppo.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://dpr.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://mmr.316326.xyz

[F02] 逐行读取文件
来源：http://rlq.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://drb.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hga.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cnb.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hvb.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wrz.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ltw.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://beg.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zrc.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://ijs.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://khn.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bmi.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ceh.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enl.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xjl.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zoe.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://uhg.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ecd.jinqigufen.top

[F04] 追加写入文件
来源：http://xex.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izt.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ccs.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://teb.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umv.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uha.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mol.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yoi.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lac.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://khw.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofm.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://nfm.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://uff.gzhubu.top


<!-- 参考信息 -->