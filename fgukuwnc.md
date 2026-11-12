代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://way.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://atg.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://jji.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://blx.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hxw.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://teo.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://toy.ivvv.top

PHP:  array_count_values($arr);
来源：http://ewm.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhq.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpk.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ygp.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://odn.c1oappe.top

Ruby: arr.tally
来源：http://qjw.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zqj.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://aag.hnxiangtu.top

Py:   x in arr
来源：http://ajh.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://box.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://euw.nanxinkj.top

TS:   arr.includes(x)
来源：http://qgf.zhengqikj.top

Java: list.contains(x)
来源：http://sru.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://abx.redwolf501.top

Ruby: arr.include?(x)
来源：http://djt.sxryk.cn

C#:   list.Contains(x)
来源：http://iab.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://glb.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lvh.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://grm.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://biy.meibo888.top

TS:   [...arr];
来源：http://nol.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://hfs.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wmb.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://hqt.ehwqpu.com

C#:   new List<int>(list);
来源：http://lsg.jqgfzy.top

[D23] reduce 累积计算
来源：http://kci.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://owq.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qqc.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://plz.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zpa.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://kyg.sysykeji.top

Go:   // 手写循环
来源：http://woy.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cbt.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gqf.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://skr.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hgd.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://syn.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yvw.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://der.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wpg.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgu.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ktq.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tct.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://nzh.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lut.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tas.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xzd.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qkp.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fta.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ycr.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://chr.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://egk.pengpengdd.cyou

[D26] 数组转字符串
来源：http://gbn.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://qlf.pycfn.com

PHP:  implode(", ", $arr);
来源：http://xlx.zhongyouzk.top

JS:   arr.join(", ")
来源：http://lza.sweek.top

TS:   arr.join(", ")
来源：http://yjb.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://pwd.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://huv.gotoacloud.top

Ruby: arr.join(", ")
来源：http://jpy.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://dmp.cashguo.top

================================================================================
来源：http://vwf.redwolf501.top

E. 字符串处理
来源：http://cqp.redwolf501.top

================================================================================
来源：http://yzs.sjlbkw.cn

[E01] 拼接字符串
来源：http://vdq.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nnq.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mbe.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://acq.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://per.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isj.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yin.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hen.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gin.c1oappe.top

[E02] 重复字符串
来源：http://xkj.yfazqb.com

Py:   "ab" * 3
来源：http://ruo.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://hjy.yfazqb.com

JS:   "ab".repeat(3)
来源：http://bhf.uphjek.com

TS:   "ab".repeat(3)
来源：http://vhx.fengsongda.top

Java: "ab".repeat(3)
来源：http://wok.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://ryi.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://nxh.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ufz.zycfv.cn

[E03] 截取子串
来源：http://cbw.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://txa.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aig.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lsj.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://mcl.xylfe.cn

Java: s.substring(1, 4)
来源：http://dzc.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kvh.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://woq.pycfn.com

C#:   s.Substring(1, 3)
来源：http://mzm.dianchejie.cn

[E04] 查找子串位置
来源：http://ujd.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://cfo.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://nkh.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zuu.yvedp.cn

TS:   s.indexOf("x")
来源：http://wdv.yanxiufei.cn

Java: s.indexOf("x")
来源：http://scq.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://vcv.fengsongda.top

Ruby: s.index("x")
来源：http://cxp.yj20258888.top

C#:   s.IndexOf("x")
来源：http://bfv.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lzc.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pye.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gzu.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gly.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vfm.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jat.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lab.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xhp.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pld.pycfn.com

[E06] 替换子串
来源：http://qfc.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wzm.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://kfl.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hlx.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://kat.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ida.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://djp.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nbt.meibo888.top

C#:   s.Replace("a", "b")
来源：http://sol.yuxming.cn

[E07] 按分隔符拆分
来源：http://hjc.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wkt.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dcs.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cjy.cqqwz.cn

TS:   s.split(",")
来源：http://drd.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rez.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lih.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://wgn.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://agl.cashguo.top

[E08] 数组按分隔符合并
来源：http://bzi.guannengcc.top

Py:   ",".join(items)
来源：http://ivf.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://yol.wangshuangyany.cn

JS:   items.join(",")
来源：http://eor.sweek.top

TS:   items.join(",")
来源：http://pwc.ppjwa.cn

Java: String.join(",", items)
来源：http://ftu.cashguo.top

Go:   strings.Join(items, ",")
来源：http://zje.cucudq.cn

Ruby: items.join(",")
来源：http://vvf.redwolf501.top

C#:   string.Join(",", items)
来源：http://qwy.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://app.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://acn.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lrb.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://ott.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://khe.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://xvf.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fuh.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xwk.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pdg.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://xyq.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aef.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xgu.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://fmt.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://vbn.sxryk.cn

Java: String.format("%03d", 7)
来源：http://gbc.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qmy.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zri.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://itg.hammf.cn

[E11] 反转字符串
来源：http://yyk.sxryk.cn

Py:   s[::-1]
来源：http://rkn.fengsongda.top

PHP:  strrev($s);
来源：http://qhx.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://qqt.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://vjz.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bjm.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oye.cashguo.top

Ruby: s.reverse
来源：http://wbh.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://fwh.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://sto.nanxuanxn.top

Py:   s.count("a")
来源：http://ycb.cheryme.top

PHP:  substr_count($s, "a");
来源：http://fmu.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://aan.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://dof.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eeb.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://crc.nanxinkj.top

Ruby: s.count("a")
来源：http://oqz.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://ujt.xylfe.cn

[E13] 逐字符遍历
来源：http://oei.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://qtc.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iml.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://sdu.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qao.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wea.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iye.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gbr.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://byb.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://ycv.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aiz.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nzd.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pnh.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kpy.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ilw.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mbs.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ujz.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://squ.feifeiyinyue.top

[E15] HTML 转义 / 反转义
来源：http://mbe.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mrk.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sdz.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yyn.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://zvw.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://otk.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fbp.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://miq.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vvk.meibo888.top

[E16] 数字千分位
来源：http://tcc.gzhubu.top

Py:   f"{1234567:,}"
来源：http://dfn.ybcxt.top

PHP:  number_format(1234567);
来源：http://clo.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hxr.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://diw.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jnl.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yjr.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bkl.cashguo.top

C#:   1234567.ToString("N0")
来源：http://hsf.ydjk.org.cn

[E17] 首字母大写
来源：http://lde.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gxq.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fsa.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uuk.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuq.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://inu.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gvf.vqdsnc.cn

Ruby: s.capitalize
来源：http://iqd.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://twx.fzhhl.top

[E18] 模板占位符替换
来源：http://myh.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gqh.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rpv.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rsa.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uex.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aps.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ebe.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fju.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ffe.yfazqb.com

[E19] 多行文本按行拆分
来源：http://qjr.shuidangran.top

Py:   s.splitlines()
来源：http://keo.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eux.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://opi.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://jte.jyoumei.cn

Java: s.lines().toList()
来源：http://bfk.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://rwi.andypj.xyz

Ruby: s.lines
来源：http://hii.epnwcf.com

C#:   s.Split('\n')
来源：http://acw.daxiang520.top

[E20] 判断字符串是否为空
来源：http://ata.xylfe.cn

Py:   if not s:
来源：http://kyk.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gwl.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uem.gaohongyu789.top

TS:   if (s === "") {}
来源：http://oxx.sweek.top

Java: if (s.isEmpty()) {}
来源：http://aia.jinqigfzy.top

Go:   if s == "" {}
来源：http://zjf.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://mqs.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yrh.nwbrower.top

[E21] 超长截断加省略号
来源：http://bwg.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbh.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eat.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsd.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fnj.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://czk.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://ptm.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://edc.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uzn.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://xqf.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvr.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ooz.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fci.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tlf.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lxh.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mad.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://asd.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mjm.tanke756.top

================================================================================
来源：http://gab.guowangkeji.top

F. 文件与目录
来源：http://rtg.svipenyu.cn

================================================================================
来源：http://ltg.cashguo.top

[F01] 读取整个文件
来源：http://hsv.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lti.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://xhd.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ulo.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fhn.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wve.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lus.sysykeji.top

Ruby: File.read("a.txt")
来源：http://qdr.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://pak.zhengqikj.top

[F02] 逐行读取文件
来源：http://wqz.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://obn.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vmt.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgy.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vih.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vvo.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iff.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://omg.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://trf.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://ozt.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpy.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gbn.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://seh.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zay.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://riq.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpq.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://qzb.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwl.daxiang520.top

[F04] 追加写入文件
来源：http://szw.hfpthk.cn


<!-- 参考信息 -->