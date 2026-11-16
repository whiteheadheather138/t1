代发 wailian999

Ruby: arr.tally
来源：http://xkt.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bhg.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://zng.tanke756.top

Py:   x in arr
来源：http://fib.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://qra.zhoulong.xyz

JS:   arr.includes(x)
来源：http://xto.hnqzz.top

TS:   arr.includes(x)
来源：http://bbz.haohaochexian.top

Java: list.contains(x)
来源：http://xco.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://qzr.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://bqz.jqgufenzy.top

C#:   list.Contains(x)
来源：http://tgg.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://mlx.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vqw.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bgr.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://puw.chenzaomai.com

TS:   [...arr];
来源：http://pdb.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://tyf.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nhy.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://dji.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://byx.uphjek.com

[D23] reduce 累积计算
来源：http://cqg.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jgz.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kxo.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://avc.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hqy.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oum.daria6918.cn

Go:   // 手写循环
来源：http://dzz.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jnq.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hah.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://lfm.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lfc.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ljm.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ezf.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zpq.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wzd.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bog.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gqu.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hpi.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://yio.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dbd.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ryn.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hmr.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eyb.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rsz.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://muo.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uli.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qwt.gaohongyu789.top

[D26] 数组转字符串
来源：http://mqz.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://kxh.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://uym.xziqi.cn

JS:   arr.join(", ")
来源：http://bwv.chenlongwang.top

TS:   arr.join(", ")
来源：http://xra.sweek.top

Java: String.join(", ", list)
来源：http://urm.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://dzx.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://bxp.hesvh.cn

C#:   string.Join(", ", list)
来源：http://wck.feifeiyinyue.top

================================================================================
来源：http://jtv.zdbjq.cn

E. 字符串处理
来源：http://qky.yvedp.cn

================================================================================
来源：http://cfk.iojbl.cn

[E01] 拼接字符串
来源：http://rif.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hch.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dhm.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzp.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cyj.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wsb.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wiy.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kvx.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mhj.hammf.cn

[E02] 重复字符串
来源：http://prj.tarul.cn

Py:   "ab" * 3
来源：http://ksd.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://gnj.mhx1999.top

JS:   "ab".repeat(3)
来源：http://chb.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://ldh.yj202588.top

Java: "ab".repeat(3)
来源：http://eho.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://zes.yj20258888.top

Ruby: "ab" * 3
来源：http://drf.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eng.xinyue.icu

[E03] 截取子串
来源：http://lph.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhg.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tta.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fig.smart0.xyz

TS:   s.slice(1, 4)
来源：http://hpt.tian-w.cn

Java: s.substring(1, 4)
来源：http://jip.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://utd.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://eaf.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://kbb.zhengqikj.top

[E04] 查找子串位置
来源：http://dwi.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://ddh.birdmap.top

PHP:  strpos($s, "x");
来源：http://eej.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ept.hcnkem.com

TS:   s.indexOf("x")
来源：http://jnu.ehwqpu.com

Java: s.indexOf("x")
来源：http://ohn.tanke756.top

Go:   strings.Index(s, "x")
来源：http://ddv.yueranfly.top

Ruby: s.index("x")
来源：http://oan.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://ael.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://slu.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://foq.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wmd.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjk.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://slu.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tlv.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dha.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://epv.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ooj.zdqjudy.top

[E06] 替换子串
来源：http://gtu.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ggx.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://mqb.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sbo.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://yda.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyi.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eax.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ajo.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://rzm.hfpthk.cn

[E07] 按分隔符拆分
来源：http://xqp.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzc.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jnl.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nfs.dashuyun.cn

TS:   s.split(",")
来源：http://bir.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://rxr.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fnp.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://orx.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qhg.gzhubu.top

[E08] 数组按分隔符合并
来源：http://mji.uphjek.com

Py:   ",".join(items)
来源：http://nwb.shuidangran.top

PHP:  implode(",", $items);
来源：http://oon.yfazqb.com

JS:   items.join(",")
来源：http://nml.sjlbkw.cn

TS:   items.join(",")
来源：http://wbx.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://yyz.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://bxb.52xcode.cn

Ruby: items.join(",")
来源：http://lia.fehbvm.com

C#:   string.Join(",", items)
来源：http://haa.xziqi.cn

[E09] 去除所有空白字符
来源：http://caa.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://snq.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vkg.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://txj.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://wbo.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://evy.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://apo.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ysp.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kxg.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://ndp.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ggq.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rva.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://lsa.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://nnw.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://xce.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zit.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zrm.epnwcf.com

[E11] 反转字符串
来源：http://ato.jlsjyb.cn

Py:   s[::-1]
来源：http://rho.ppjwa.cn

PHP:  strrev($s);
来源：http://etj.yonumen.top

JS:   [...s].reverse().join("")
来源：http://gqb.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://hvt.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zsv.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jdg.xinyue.icu

Ruby: s.reverse
来源：http://qik.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://vom.vehdjk.com

[E12] 统计某字符出现次数
来源：http://exl.yanxiufei.cn

Py:   s.count("a")
来源：http://sxq.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://oka.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://rqu.sysykeji.top

TS:   s.split("a").length - 1
来源：http://eiw.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wpy.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://pmm.gogol.net.cn

Ruby: s.count("a")
来源：http://jlx.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://yks.mhx1999.top

[E13] 逐字符遍历
来源：http://uui.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://vhh.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://unx.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nkl.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rzo.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uvt.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqv.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zmu.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ggt.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://qep.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rwz.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfk.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nyc.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fij.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zeq.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nmn.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zfa.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qgq.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://nxu.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ztb.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fzg.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zzd.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qis.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dvd.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dkb.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qgd.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://win.mhx1999.top

[E16] 数字千分位
来源：http://bte.yvedp.cn

Py:   f"{1234567:,}"
来源：http://ciy.yongpay.top

PHP:  number_format(1234567);
来源：http://dss.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nll.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fet.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxq.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://edc.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fca.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://pja.jinqigufen.top

[E17] 首字母大写
来源：http://nwz.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wtn.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://qff.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzn.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnc.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwe.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://keu.9152youxi.cn

Ruby: s.capitalize
来源：http://mkd.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zif.yanxiufei.cn

[E18] 模板占位符替换
来源：http://lhq.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zcm.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wdr.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://okd.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://awj.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rmp.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ndm.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ona.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ogn.yj20258.top

[E19] 多行文本按行拆分
来源：http://klj.hcnkem.com

Py:   s.splitlines()
来源：http://gmi.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zza.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://dvy.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://aii.birdmap.top

Java: s.lines().toList()
来源：http://cwz.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://eam.cheryme.top

Ruby: s.lines
来源：http://lpc.zhijiandao.cn

C#:   s.Split('\n')
来源：http://yby.hnqzz.top

[E20] 判断字符串是否为空
来源：http://yfn.nwbrower.top

Py:   if not s:
来源：http://uxf.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pix.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://udk.ydzc1.top

TS:   if (s === "") {}
来源：http://bcz.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://kom.zhixingplan.top

Go:   if s == "" {}
来源：http://dew.hywenlv.cn

Ruby: if s.empty?
来源：http://wjg.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eqo.hcnkem.com

[E21] 超长截断加省略号
来源：http://ryz.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sen.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ggm.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qfa.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vxn.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ecs.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://usy.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tdz.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://veu.yueranfly.top

[E22] 字节长度与字符长度
来源：http://anw.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://udj.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://syc.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mfo.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wxg.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pfw.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lbw.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://myt.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ltm.smart0.xyz

================================================================================
来源：http://igj.cucudq.cn

F. 文件与目录
来源：http://fhr.jqgufenzy.top

================================================================================
来源：http://zuy.cashguo.top

[F01] 读取整个文件
来源：http://sfk.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qoa.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://qun.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jej.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjn.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://clv.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xxc.iojbl.cn

Ruby: File.read("a.txt")
来源：http://flu.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://dgc.hysaishi.cn

[F02] 逐行读取文件
来源：http://jom.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hid.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hzw.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nyk.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jnp.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dcb.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hif.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqb.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rnr.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://yaw.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://udr.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xqx.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://peb.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnp.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ytn.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rvm.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://pwg.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dmr.tian-w.cn

[F04] 追加写入文件
来源：http://jpj.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wxp.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mbd.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://num.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wze.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wah.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://clp.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://asu.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bhc.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://ttl.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qhj.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://unq.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://wge.zhiwuduotai.top


<!-- 参考信息 -->