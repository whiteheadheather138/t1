代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ymx.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uyo.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fvg.sxryk.cn

Go:   // 手写 map[T]int
来源：http://lvf.feifeiyinyue.top

Ruby: arr.tally
来源：http://ysm.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wlz.yueranfly.top

[D21] 判断是否包含某元素
来源：http://spg.jinyuanbaomall.cn

Py:   x in arr
来源：http://dqg.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://kpm.shuidangran.top

JS:   arr.includes(x)
来源：http://jzo.chenzaomai.com

TS:   arr.includes(x)
来源：http://rpx.ehwqpu.com

Java: list.contains(x)
来源：http://qms.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://znl.havefunace.top

Ruby: arr.include?(x)
来源：http://uue.tarul.cn

C#:   list.Contains(x)
来源：http://ncb.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://qno.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://szg.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://upr.zycfv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tyo.yuanzhike.top

TS:   [...arr];
来源：http://hrw.andypj.xyz

Java: new ArrayList<>(list);
来源：http://zvy.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://csz.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://sho.wangdashe.top

C#:   new List<int>(list);
来源：http://erw.jiagoushi.top

[D23] reduce 累积计算
来源：http://kyr.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tni.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vht.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izm.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jzg.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lym.ydjk.org.cn

Go:   // 手写循环
来源：http://rkw.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ksj.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eom.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://ipm.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ylp.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ptw.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nst.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rct.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lix.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ich.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://swk.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdr.ivvv.top

[D25] Set 集合去重与交并差
来源：http://uak.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmj.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bwi.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mcy.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jgf.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cpi.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vca.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bbk.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qiw.epnwcf.com

[D26] 数组转字符串
来源：http://oud.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://ipo.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://bog.bjfxy.top

JS:   arr.join(", ")
来源：http://doc.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://ytn.cqqwz.cn

Java: String.join(", ", list)
来源：http://zqi.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://oba.yj20258888.top

Ruby: arr.join(", ")
来源：http://enj.c1oappe.top

C#:   string.Join(", ", list)
来源：http://ylv.sysykeji.top

================================================================================
来源：http://tqk.shangyingyoupin.top

E. 字符串处理
来源：http://zvc.bjfxy.top

================================================================================
来源：http://irk.52xcode.cn

[E01] 拼接字符串
来源：http://wyq.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tjj.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ozu.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uax.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aas.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opr.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hof.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jtm.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yjd.yfazqb.com

[E02] 重复字符串
来源：http://fhg.cheryme.top

Py:   "ab" * 3
来源：http://eim.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://jub.sysykeji.top

JS:   "ab".repeat(3)
来源：http://rua.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://zaa.yj20258.top

Java: "ab".repeat(3)
来源：http://vgr.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://qdd.kuanghao11.cn

Ruby: "ab" * 3
来源：http://qfc.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cly.jqgufenzy.top

[E03] 截取子串
来源：http://quw.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nig.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bhq.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbj.zycfv.cn

TS:   s.slice(1, 4)
来源：http://rbq.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://fcu.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nko.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://gdw.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://vpq.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://iav.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://rha.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://dph.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tkm.yj20258.top

TS:   s.indexOf("x")
来源：http://nqw.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://gwk.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://pqu.nanxinkj.top

Ruby: s.index("x")
来源：http://dms.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://fld.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nfu.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vbd.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kzz.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nib.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://fxm.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efe.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bzj.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rhp.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ika.fehbvm.com

[E06] 替换子串
来源：http://ene.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dvc.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://zdn.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxl.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://evl.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kuz.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cry.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mco.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://qfl.aibaodan.cn

[E07] 按分隔符拆分
来源：http://owa.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://atr.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kkp.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hxr.wangshuangyany.cn

TS:   s.split(",")
来源：http://wjh.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tnb.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ryw.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://xtg.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wuz.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://bbv.cucudq.cn

Py:   ",".join(items)
来源：http://vup.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://wcy.jqgufenzy.top

JS:   items.join(",")
来源：http://fuz.bbcook.cn

TS:   items.join(",")
来源：http://xgh.ybcxt.top

Java: String.join(",", items)
来源：http://oup.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://hgx.cheryme.top

Ruby: items.join(",")
来源：http://vvj.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://emd.daxiang520.top

[E09] 去除所有空白字符
来源：http://myf.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nki.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pib.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wof.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://zli.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://poc.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyh.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://opy.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofw.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://thd.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpr.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ryv.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://fce.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://qmo.birdmap.top

Java: String.format("%03d", 7)
来源：http://ebw.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wra.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iwz.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://caj.shzxlz.cn

[E11] 反转字符串
来源：http://llq.xinyue.icu

Py:   s[::-1]
来源：http://tfa.52xcode.cn

PHP:  strrev($s);
来源：http://zkn.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://gih.hammf.cn

TS:   [...s].reverse().join("")
来源：http://mmu.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dzf.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ohj.nanxinkj.top

Ruby: s.reverse
来源：http://bss.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://yfc.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://jvx.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://kxg.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://din.ivvv.top

JS:   s.split("a").length - 1
来源：http://bid.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://pzg.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pqh.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://bcq.yuxming.cn

Ruby: s.count("a")
来源：http://iaj.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://wsx.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://tzx.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://kkr.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zha.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tfy.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://afh.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brt.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fgt.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://upq.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ayn.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://oje.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sye.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ird.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnz.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nki.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cde.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ptm.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cxu.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://izt.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://dfb.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gnp.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zqt.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rwb.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hcp.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kbm.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vug.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbt.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yyp.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://oze.ybcxt.top

Py:   f"{1234567:,}"
来源：http://dlo.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://jmi.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rnb.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qet.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ttu.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dti.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hts.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://gwt.svipenyu.cn

[E17] 首字母大写
来源：http://eub.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iga.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ptv.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://smu.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vdc.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fgi.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://csh.sxryk.cn

Ruby: s.capitalize
来源：http://osc.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://irz.ydzc1.top

[E18] 模板占位符替换
来源：http://idt.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mxs.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfp.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hcw.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://oei.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ejd.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hsz.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zzk.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uky.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://kio.yj20258888.top

Py:   s.splitlines()
来源：http://ttk.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ksx.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://kzi.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://xfz.shuidangran.top

Java: s.lines().toList()
来源：http://xpj.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://ewm.wangdashe.top

Ruby: s.lines
来源：http://cty.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://liy.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://vlf.jyoumei.cn

Py:   if not s:
来源：http://sxy.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lfb.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://klo.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://qba.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://mrd.shangyingyoupin.top

Go:   if s == "" {}
来源：http://tog.zhiwuduotai.top

Ruby: if s.empty?
来源：http://hqt.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lyr.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://cts.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://klg.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vyy.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqc.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsm.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xka.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://rae.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omr.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fsf.uphjek.com

[E22] 字节长度与字符长度
来源：http://uhu.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ihx.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kkl.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fau.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbu.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hwo.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rzc.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://lpa.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zok.hongshengwenyu.top

================================================================================
来源：http://lbe.shanyushiyangtech.top

F. 文件与目录
来源：http://bti.gogol.net.cn

================================================================================
来源：http://uip.yonumen.top

[F01] 读取整个文件
来源：http://uup.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aiu.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://acz.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vaq.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fmz.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://tkr.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mkv.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://kwv.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://drt.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://zwm.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctj.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hsv.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpl.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktc.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fad.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iuz.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sqm.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zsa.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://dne.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://stt.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cjf.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qer.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukc.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yqv.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pve.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://dep.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ccz.jqgfzy.top

[F04] 追加写入文件
来源：http://sug.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pad.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pma.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fds.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ltp.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xwo.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tuf.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kao.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vyb.nwbrower.top


<!-- 参考信息 -->