代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://xfk.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ykw.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://mfx.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyx.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ewk.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://hwa.yfazqb.com

Py:   Counter(arr)
来源：http://atj.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://mpb.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkc.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zhd.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://akz.fktsv.cn

Go:   // 手写 map[T]int
来源：http://vfb.hnxiangtu.top

Ruby: arr.tally
来源：http://vkt.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ntt.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://rhi.hcnkem.com

Py:   x in arr
来源：http://wlv.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://ayx.hcnkem.com

JS:   arr.includes(x)
来源：http://fin.52xcode.cn

TS:   arr.includes(x)
来源：http://psw.jlsjyb.cn

Java: list.contains(x)
来源：http://jsi.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://txo.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://afs.yonumen.top

C#:   list.Contains(x)
来源：http://kqv.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://ogy.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qdo.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fjg.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qme.sjlbkw.cn

TS:   [...arr];
来源：http://ewd.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://bgw.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wql.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://lys.cashguo.top

C#:   new List<int>(list);
来源：http://vwv.redwolf501.top

[D23] reduce 累积计算
来源：http://kvi.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pob.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swa.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gpv.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpe.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dzo.nwbrower.top

Go:   // 手写循环
来源：http://azx.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ehp.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eci.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://gyy.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvo.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cbe.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flu.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qin.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ipd.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jnx.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xet.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cob.hammf.cn

[D25] Set 集合去重与交并差
来源：http://tkx.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://reb.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ozz.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kez.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dak.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://amx.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mca.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iwb.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yoa.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://ewx.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://wof.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://atl.pycfn.com

JS:   arr.join(", ")
来源：http://fcv.cdnleiting.top

TS:   arr.join(", ")
来源：http://tid.zycfv.cn

Java: String.join(", ", list)
来源：http://tnv.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://tdw.yfazqb.com

Ruby: arr.join(", ")
来源：http://yio.fehbvm.com

C#:   string.Join(", ", list)
来源：http://grh.birdmap.top

================================================================================
来源：http://qub.ctjpmb.com

E. 字符串处理
来源：http://kzj.gogol.net.cn

================================================================================
来源：http://oow.aibaodan.cn

[E01] 拼接字符串
来源：http://ghs.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ahf.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hkq.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnt.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rye.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ztz.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dfn.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhv.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uyb.0kj1m.cn

[E02] 重复字符串
来源：http://bzs.52xcode.cn

Py:   "ab" * 3
来源：http://jed.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://hui.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://rnm.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://aay.jqgfzy.top

Java: "ab".repeat(3)
来源：http://xiz.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://pch.ydjk.org.cn

Ruby: "ab" * 3
来源：http://glv.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qny.shangyingyoupin.top

[E03] 截取子串
来源：http://xdh.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wii.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jmp.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ahi.yvedp.cn

TS:   s.slice(1, 4)
来源：http://jmc.daxiang520.top

Java: s.substring(1, 4)
来源：http://wbj.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nze.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://xxh.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://rcj.svipenyu.cn

[E04] 查找子串位置
来源：http://uby.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://mvz.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://lde.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngf.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://xbk.pycfn.com

Java: s.indexOf("x")
来源：http://pvo.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://hdc.fktsv.cn

Ruby: s.index("x")
来源：http://our.yuxming.cn

C#:   s.IndexOf("x")
来源：http://nfr.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://trt.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pyg.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://azy.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efw.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://feu.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uto.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zac.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yuy.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dtf.wangshuangyany.cn

[E06] 替换子串
来源：http://pjw.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mrh.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://whe.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fyy.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://nwf.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxv.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hdf.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jpb.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://ghe.hfpthk.cn

[E07] 按分隔符拆分
来源：http://hgk.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mpg.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://muz.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gnf.fanxiaobao.xyz

TS:   s.split(",")
来源：http://cvs.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://wnb.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ryk.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://rsg.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zno.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://ukf.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://npz.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://gwt.cucudq.cn

JS:   items.join(",")
来源：http://uir.gzhubu.top

TS:   items.join(",")
来源：http://vtl.tianlin.xyz

Java: String.join(",", items)
来源：http://mcj.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://tbr.zhijiandao.cn

Ruby: items.join(",")
来源：http://znc.guowangkeji.top

C#:   string.Join(",", items)
来源：http://gpx.svipenyu.cn

[E09] 去除所有空白字符
来源：http://tls.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lzl.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://crn.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://omn.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://yxt.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://kqq.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lnl.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ohx.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jqi.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://zvw.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://esb.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hku.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://shg.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://zmm.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://hbs.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ivh.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jqd.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wqk.xylfe.cn

[E11] 反转字符串
来源：http://ocl.feifeiyinyue.top

Py:   s[::-1]
来源：http://vhu.chenjidiqi.icu

PHP:  strrev($s);
来源：http://vbu.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://gml.uphjek.com

TS:   [...s].reverse().join("")
来源：http://cih.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://llc.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://adk.shuidangran.top

Ruby: s.reverse
来源：http://vcb.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jiz.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://yyn.dianchejie.cn

Py:   s.count("a")
来源：http://fye.yj202588.top

PHP:  substr_count($s, "a");
来源：http://zev.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://lde.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://rcm.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rki.316326.xyz

Go:   strings.Count(s, "a")
来源：http://rlf.zdbjq.cn

Ruby: s.count("a")
来源：http://joo.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://ugh.haohaochexian.top

[E13] 逐字符遍历
来源：http://zgn.tanke756.top

Py:   for ch in s: print(ch)
来源：http://hmh.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dlv.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ggx.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ycn.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xzp.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qro.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ihs.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tqf.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://lop.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blm.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvo.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://giw.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ofp.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://stq.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmw.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fbr.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tkl.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://rti.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eeg.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xmy.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://erh.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qsp.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fbt.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cgz.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zul.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sdo.sweek.top

[E16] 数字千分位
来源：http://dxk.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://aps.bjfxy.top

PHP:  number_format(1234567);
来源：http://fgd.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yma.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fdj.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://trk.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qfk.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfo.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://brb.shzxlz.cn

[E17] 首字母大写
来源：http://xeq.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nyd.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hpb.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hjy.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://inf.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://urk.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzg.cheryme.top

Ruby: s.capitalize
来源：http://ldh.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwe.redwolf501.top

[E18] 模板占位符替换
来源：http://ldj.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eeh.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sjc.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kbo.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://avb.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yma.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kwk.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cia.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nme.bjfxy.top

[E19] 多行文本按行拆分
来源：http://tsy.vqdsnc.cn

Py:   s.splitlines()
来源：http://rio.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eak.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://pag.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://twb.zycfv.cn

Java: s.lines().toList()
来源：http://jic.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://doi.xylfe.cn

Ruby: s.lines
来源：http://mfe.kuanghao11.cn

C#:   s.Split('\n')
来源：http://shl.316326.xyz

[E20] 判断字符串是否为空
来源：http://btl.redwolf501.top

Py:   if not s:
来源：http://vhc.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vcn.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tuo.xuanzx.com

TS:   if (s === "") {}
来源：http://nze.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://dez.sysykeji.top

Go:   if s == "" {}
来源：http://xna.haohaochexian.top

Ruby: if s.empty?
来源：http://tov.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rzm.nanxinkj.top

[E21] 超长截断加省略号
来源：http://hls.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pqk.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gmj.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xql.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztw.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ldd.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://leg.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vqj.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xrb.mhx1999.top

[E22] 字节长度与字符长度
来源：http://kbx.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tip.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxs.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlj.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pcz.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exw.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fbf.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://mlz.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kpf.kuanghao11.cn

================================================================================
来源：http://ltn.dashuyun.cn

F. 文件与目录
来源：http://wmq.hammf.cn

================================================================================
来源：http://gex.hnxiangtu.top

[F01] 读取整个文件
来源：http://kja.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vqh.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://ngb.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ise.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hrp.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rxv.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pln.aizwys.cn

Ruby: File.read("a.txt")
来源：http://yqa.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://mks.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://alf.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nzo.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gah.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://obh.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xmq.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wop.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rxs.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bmh.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cfh.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://lrp.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bhn.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://egi.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jhh.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yng.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pjw.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cya.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://qbl.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdo.iojbl.cn

[F04] 追加写入文件
来源：http://lbr.cheryme.top


<!-- 参考信息 -->