代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vpy.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://sng.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://jlr.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://zxi.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gco.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gyl.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xiu.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://jnm.andypj.xyz

Ruby: arr.tally
来源：http://gli.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jbh.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://hyo.tianlin.xyz

Py:   x in arr
来源：http://qra.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://nzo.guannengcc.top

JS:   arr.includes(x)
来源：http://qzr.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://jmo.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://ugf.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://dtw.sxryk.cn

Ruby: arr.include?(x)
来源：http://fiz.ctjpmb.com

C#:   list.Contains(x)
来源：http://mhq.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://xkw.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hkz.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vgm.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pql.yangfankeji.com

TS:   [...arr];
来源：http://cxd.iojbl.cn

Java: new ArrayList<>(list);
来源：http://cmj.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cym.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://pqo.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://ymv.xuanzx.com

[D23] reduce 累积计算
来源：http://arl.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jry.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://onx.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfp.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jrg.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dcd.hysaishi.cn

Go:   // 手写循环
来源：http://lga.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zbt.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nin.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://zed.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zvd.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://scw.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://drb.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://faz.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hfk.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dyl.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jso.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pzw.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://eta.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://myh.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mje.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sdd.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dhg.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xxd.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wue.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pax.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fwu.0kj1m.cn

[D26] 数组转字符串
来源：http://pxz.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://ggr.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://mxz.cheryme.top

JS:   arr.join(", ")
来源：http://vlf.hfpthk.cn

TS:   arr.join(", ")
来源：http://gik.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://ion.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://fyc.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://wlc.hesvh.cn

C#:   string.Join(", ", list)
来源：http://sqv.meibo888.top

================================================================================
来源：http://tjw.guowangkeji.top

E. 字符串处理
来源：http://cbj.cucudq.cn

================================================================================
来源：http://hkk.cqqwz.cn

[E01] 拼接字符串
来源：http://bev.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fpf.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nch.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://klv.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfl.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qrx.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qbl.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ewt.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://plj.jinghuilouyu.cn

[E02] 重复字符串
来源：http://bnh.hysaishi.cn

Py:   "ab" * 3
来源：http://jsl.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://qlf.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://wby.zycfv.cn

TS:   "ab".repeat(3)
来源：http://jpy.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://xea.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://ani.yueranfly.top

Ruby: "ab" * 3
来源：http://dpc.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mvk.sysykeji.top

[E03] 截取子串
来源：http://ead.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgd.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jtt.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wsq.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://krq.cdnleiting.top

Java: s.substring(1, 4)
来源：http://zcg.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yun.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://smb.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://ich.guowangkeji.top

[E04] 查找子串位置
来源：http://dfx.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://jwh.hammf.cn

PHP:  strpos($s, "x");
来源：http://yti.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fdt.jiagoushi.top

TS:   s.indexOf("x")
来源：http://wpp.havefunace.top

Java: s.indexOf("x")
来源：http://ive.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://utx.xziqi.cn

Ruby: s.index("x")
来源：http://cqm.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://znx.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qqb.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wtz.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://byq.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dtt.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://omt.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agh.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mdt.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ofa.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://skt.yuanzhike.top

[E06] 替换子串
来源：http://ovn.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zhc.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://vlk.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztd.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://uld.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://udg.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ave.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qap.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://rut.52xcode.cn

[E07] 按分隔符拆分
来源：http://hxm.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tul.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yal.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqs.hywenlv.cn

TS:   s.split(",")
来源：http://cpl.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://sxs.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zqs.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://ocl.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sje.epnwcf.com

[E08] 数组按分隔符合并
来源：http://uxu.bjfxy.top

Py:   ",".join(items)
来源：http://emd.xinyue.icu

PHP:  implode(",", $items);
来源：http://wfz.cheryme.top

JS:   items.join(",")
来源：http://cgx.hnxiangtu.top

TS:   items.join(",")
来源：http://xse.guowangkeji.top

Java: String.join(",", items)
来源：http://agu.cheryme.top

Go:   strings.Join(items, ",")
来源：http://ams.guannengcc.top

Ruby: items.join(",")
来源：http://ahy.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://qqb.shuidangran.top

[E09] 去除所有空白字符
来源：http://gwi.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eqd.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hji.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://dnz.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://kvv.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://onb.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xdq.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://gxs.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ehg.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://sdu.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zhx.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mbv.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://mkv.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://wdv.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://oez.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vsk.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kbx.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vmp.9152youxi.cn

[E11] 反转字符串
来源：http://yzx.yueranfly.top

Py:   s[::-1]
来源：http://sff.gogol.net.cn

PHP:  strrev($s);
来源：http://tpu.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://jol.uphjek.com

TS:   [...s].reverse().join("")
来源：http://qrz.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dtv.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmt.zhoulong.xyz

Ruby: s.reverse
来源：http://nac.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jyj.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://yjy.snrcjt.cn

Py:   s.count("a")
来源：http://par.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://zuy.fehbvm.com

JS:   s.split("a").length - 1
来源：http://bth.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://fbg.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mba.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://yav.xziqi.cn

Ruby: s.count("a")
来源：http://evn.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://gqb.ehwqpu.com

[E13] 逐字符遍历
来源：http://ydl.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://ddg.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hwf.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kbm.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vhu.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axd.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kpi.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nsl.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ngt.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://gbl.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eoj.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qig.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://trk.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvk.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nqr.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ivi.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bmt.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ede.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://cxi.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mdf.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://asm.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxm.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vts.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jyd.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://naw.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bqd.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kgz.xuetiantiany.cn

[E16] 数字千分位
来源：http://iou.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://ayv.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://hyf.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://sth.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yfw.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bsk.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sni.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://utf.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://zls.gaohongyu789.top

[E17] 首字母大写
来源：http://jue.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lrz.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xik.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsy.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dgx.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bst.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://per.nwbrower.top

Ruby: s.capitalize
来源：http://mbi.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojo.gaohongyu789.top

[E18] 模板占位符替换
来源：http://pbm.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ybe.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://spa.sweek.top

JS:   tpl.replaceAll("{name}", name)
来源：http://amv.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tyw.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hyj.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qwh.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lrw.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dao.shuidangran.top

[E19] 多行文本按行拆分
来源：http://kmf.yvedp.cn

Py:   s.splitlines()
来源：http://xpx.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kma.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://gxq.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://rak.hfpthk.cn

Java: s.lines().toList()
来源：http://jzy.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://mtq.quarkkingdee.top

Ruby: s.lines
来源：http://qdh.gzhubu.top

C#:   s.Split('\n')
来源：http://tha.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://lry.9152youxi.cn

Py:   if not s:
来源：http://pfj.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qaf.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lvb.uphjek.com

TS:   if (s === "") {}
来源：http://ork.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://fas.tanke756.top

Go:   if s == "" {}
来源：http://uxg.yangfankeji.com

Ruby: if s.empty?
来源：http://cxd.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qzn.fehbvm.com

[E21] 超长截断加省略号
来源：http://sup.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lyz.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://csf.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxh.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mjf.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xbc.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://dpd.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lqe.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dzn.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://jth.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qqp.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxw.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vmx.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qol.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sef.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rxc.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://tyr.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htb.havefunace.top

================================================================================
来源：http://bhb.snrcjt.cn

F. 文件与目录
来源：http://tan.vqdsnc.cn

================================================================================
来源：http://llx.yj202588.top

[F01] 读取整个文件
来源：http://yrj.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ttf.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://kpb.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://twa.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dep.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://noh.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nwl.wangdashe.top

Ruby: File.read("a.txt")
来源：http://zdz.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://tcx.yvedp.cn

[F02] 逐行读取文件
来源：http://ira.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uhn.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nnx.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://btv.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dtc.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bjq.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vgq.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nhs.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ikj.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://vqx.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qbh.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qca.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kmm.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxe.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rla.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tsp.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://zsz.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vse.yfazqb.com

[F04] 追加写入文件
来源：http://kjv.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lwh.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vmd.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lyb.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ull.shangyingyoupin.top


<!-- 参考信息 -->