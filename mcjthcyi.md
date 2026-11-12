代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://zav.shzxlz.cn

JS:   arr.includes(x)
来源：http://ahy.cheryme.top

TS:   arr.includes(x)
来源：http://pay.guowangkeji.top

Java: list.contains(x)
来源：http://btn.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://zjx.cheryme.top

Ruby: arr.include?(x)
来源：http://mom.yonumen.top

C#:   list.Contains(x)
来源：http://clv.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://yxi.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://etp.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wxa.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gsv.bbcook.cn

TS:   [...arr];
来源：http://qrd.zycfv.cn

Java: new ArrayList<>(list);
来源：http://meo.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vdl.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://mvm.cheryme.top

C#:   new List<int>(list);
来源：http://lsm.mhx1999.top

[D23] reduce 累积计算
来源：http://jkz.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gyy.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gvt.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wtz.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oke.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mtd.316326.xyz

Go:   // 手写循环
来源：http://qwn.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zeh.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jme.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://vey.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://grn.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cyx.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://anm.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://unu.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://meg.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uvt.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdt.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://evd.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://yeb.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://olc.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tam.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ywt.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ppb.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oju.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mzx.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jwr.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://geg.fzhhl.top

[D26] 数组转字符串
来源：http://tgu.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://dzf.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://jfz.tian-w.cn

JS:   arr.join(", ")
来源：http://sqo.pycfn.com

TS:   arr.join(", ")
来源：http://ews.dashuyun.cn

Java: String.join(", ", list)
来源：http://ign.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://owq.zhengqikj.top

Ruby: arr.join(", ")
来源：http://hzi.pycfn.com

C#:   string.Join(", ", list)
来源：http://fns.shanyushiyangkeji.top

================================================================================
来源：http://xpz.jinyuanbaomall.cn

E. 字符串处理
来源：http://czn.yangfankeji.com

================================================================================
来源：http://nrm.shuidangran.top

[E01] 拼接字符串
来源：http://txz.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fch.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qxi.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lop.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lcu.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://svk.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cgh.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iru.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ajb.gotoacloud.top

[E02] 重复字符串
来源：http://tsc.shzxlz.cn

Py:   "ab" * 3
来源：http://dxs.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://ftb.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://lnn.smart0.xyz

TS:   "ab".repeat(3)
来源：http://wsc.wangdashe.top

Java: "ab".repeat(3)
来源：http://alt.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://szc.gogol.net.cn

Ruby: "ab" * 3
来源：http://kck.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jjl.yfazqb.com

[E03] 截取子串
来源：http://fxo.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://djs.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://peu.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dmv.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://rfb.tianlin.xyz

Java: s.substring(1, 4)
来源：http://ndk.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mxs.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://zrw.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://xbn.sysykeji.top

[E04] 查找子串位置
来源：http://sai.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://gvp.fzhhl.top

PHP:  strpos($s, "x");
来源：http://uqe.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dvh.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://yck.guowangkeji.top

Java: s.indexOf("x")
来源：http://zjl.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://uuh.jqgufenzy.top

Ruby: s.index("x")
来源：http://sos.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://xas.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hdv.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lkk.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vgg.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zuj.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jna.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iyp.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yir.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pox.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqo.daria6918.cn

[E06] 替换子串
来源：http://lom.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://clz.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://ibo.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jod.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://rpi.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lhi.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://igf.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://roe.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://him.chenzaomai.com

[E07] 按分隔符拆分
来源：http://wsb.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fyh.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nnl.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lbs.shangyingyoupin.top

TS:   s.split(",")
来源：http://tym.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://uzc.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dpa.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://eii.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hkb.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://sux.0kj1m.cn

Py:   ",".join(items)
来源：http://jvc.ppjwa.cn

PHP:  implode(",", $items);
来源：http://nhd.vqdsnc.cn

JS:   items.join(",")
来源：http://nao.nanxinkj.top

TS:   items.join(",")
来源：http://wej.316326.xyz

Java: String.join(",", items)
来源：http://ggf.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://zqz.jyoumei.cn

Ruby: items.join(",")
来源：http://unu.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://iax.havefunace.top

[E09] 去除所有空白字符
来源：http://qii.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lmo.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ucu.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://rmo.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://dhb.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://tfs.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vln.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://rrk.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://spb.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://may.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://irr.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hrw.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://tpw.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://taz.cheryme.top

Java: String.format("%03d", 7)
来源：http://qfy.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://oop.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://add.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://igg.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://hhf.pengpengdd.cyou

Py:   s[::-1]
来源：http://wom.andypj.xyz

PHP:  strrev($s);
来源：http://sca.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://apg.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://jpz.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bki.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bso.hcnkem.com

Ruby: s.reverse
来源：http://beo.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ypp.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://isf.yueranfly.top

Py:   s.count("a")
来源：http://smu.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://ytr.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://bzg.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://snu.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ktj.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://prx.havefunace.top

Ruby: s.count("a")
来源：http://qbl.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://kst.zhongyouzk.top

[E13] 逐字符遍历
来源：http://tyo.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://tzb.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lfu.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://odr.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dmn.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fla.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cac.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kro.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sqi.fktsv.cn

[E14] URL 编码与 Base64
来源：http://dvs.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://stj.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lvo.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dko.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xgz.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wlv.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ekn.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://btn.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fjh.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://kci.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xks.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpb.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ney.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kfa.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kko.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hro.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fcl.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vif.zdbjq.cn

[E16] 数字千分位
来源：http://pty.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://pnj.sysykeji.top

PHP:  number_format(1234567);
来源：http://fao.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://yez.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hoj.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qrh.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vzo.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hek.tarul.cn

C#:   1234567.ToString("N0")
来源：http://sbo.ybcxt.top

[E17] 首字母大写
来源：http://xbd.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tgc.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tjs.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mnj.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpj.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://stk.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ihw.yvedp.cn

Ruby: s.capitalize
来源：http://zjd.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jdb.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://sxo.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ekg.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://scf.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nki.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nbr.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nlc.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gym.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oxa.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://evh.cheryme.top

[E19] 多行文本按行拆分
来源：http://mxx.cucudq.cn

Py:   s.splitlines()
来源：http://huz.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lpn.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://zku.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://alt.xuanzx.com

Java: s.lines().toList()
来源：http://swo.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://ase.yj20258.top

Ruby: s.lines
来源：http://ull.sweek.top

C#:   s.Split('\n')
来源：http://ugs.xylfe.cn

[E20] 判断字符串是否为空
来源：http://ife.uphjek.com

Py:   if not s:
来源：http://azv.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lxt.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://haz.haohaochexian.top

TS:   if (s === "") {}
来源：http://fsd.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://ilc.shuidangran.top

Go:   if s == "" {}
来源：http://gya.snrcjt.cn

Ruby: if s.empty?
来源：http://icu.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ppc.hywenlv.cn

[E21] 超长截断加省略号
来源：http://naw.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mdj.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ahq.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogg.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpx.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://elg.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://jzn.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wlk.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vlv.xuanzx.com

[E22] 字节长度与字符长度
来源：http://avx.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fgx.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbi.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpg.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nes.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yso.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ngc.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://dsi.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zln.ywan-chungtsiang.top

================================================================================
来源：http://ckb.vehdjk.com

F. 文件与目录
来源：http://vic.ywan-chungtsiang.top

================================================================================
来源：http://ael.tian-w.cn

[F01] 读取整个文件
来源：http://tam.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uko.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://ytq.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nok.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uif.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://spb.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vso.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://pbz.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://sbt.fktsv.cn

[F02] 逐行读取文件
来源：http://kqw.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nqq.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mbt.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://guu.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wgo.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tka.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://prs.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vgi.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xwz.pycfn.com

[F03] 写入文件（覆盖）
来源：http://ipf.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fwp.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mwy.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhr.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfr.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://irf.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yvz.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://hba.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wyl.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://lno.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fws.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jub.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqr.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jla.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tpd.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rew.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wmc.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ifm.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://twu.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mpu.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://wdm.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://yyu.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://jlw.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vot.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kfq.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://oyz.andypj.xyz


<!-- 参考信息 -->