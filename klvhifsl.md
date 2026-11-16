代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://eue.shuidangran.top

Ruby: arr.include?(x)
来源：http://rhw.yj20258.top

C#:   list.Contains(x)
来源：http://jqs.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://sjj.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wqd.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pwi.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hkv.ctjpmb.com

TS:   [...arr];
来源：http://mej.yueranfly.top

Java: new ArrayList<>(list);
来源：http://wzy.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://rxi.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://sab.sweek.top

C#:   new List<int>(list);
来源：http://qtx.wangdashe.top

[D23] reduce 累积计算
来源：http://tgu.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vdb.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wbq.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyd.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vim.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qoe.dianchejie.cn

Go:   // 手写循环
来源：http://bfu.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tqx.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zsb.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://ozy.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nhv.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dlv.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hzr.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://omh.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rvh.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zrn.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pge.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://icm.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://ynm.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://knd.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xid.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://atp.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://olz.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qfj.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tlz.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xcv.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cfa.hongshengwenyu.top

[D26] 数组转字符串
来源：http://upg.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://fjj.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://sst.zhoulong.xyz

JS:   arr.join(", ")
来源：http://zru.fehbvm.com

TS:   arr.join(", ")
来源：http://ofq.fengsongda.top

Java: String.join(", ", list)
来源：http://dwb.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://bmx.aibaodan.cn

Ruby: arr.join(", ")
来源：http://ail.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://rot.jlsjyb.cn

================================================================================
来源：http://cko.shanyushiyangtech.top

E. 字符串处理
来源：http://aew.cdnleiting.top

================================================================================
来源：http://ynd.fehbvm.com

[E01] 拼接字符串
来源：http://sci.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bih.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mtp.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vuy.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vom.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gsg.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvk.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://whn.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wrm.aibaodan.cn

[E02] 重复字符串
来源：http://glv.xziqi.cn

Py:   "ab" * 3
来源：http://dmk.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://vhn.ybcxt.top

JS:   "ab".repeat(3)
来源：http://uwg.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://bea.ctjpmb.com

Java: "ab".repeat(3)
来源：http://awz.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://dor.kuanghao11.cn

Ruby: "ab" * 3
来源：http://wpl.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qcb.fzhhl.top

[E03] 截取子串
来源：http://jgq.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://crf.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ifk.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ogm.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://urk.hfpthk.cn

Java: s.substring(1, 4)
来源：http://roy.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aom.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://rnv.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://znt.gzhubu.top

[E04] 查找子串位置
来源：http://ytg.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://zhp.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://agr.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://krg.cucudq.cn

TS:   s.indexOf("x")
来源：http://cyk.mhx1999.top

Java: s.indexOf("x")
来源：http://lij.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://rjg.birdmap.top

Ruby: s.index("x")
来源：http://uis.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://dyj.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jze.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oeo.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ars.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cua.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ygk.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oix.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hfb.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jil.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cls.shzxlz.cn

[E06] 替换子串
来源：http://ohk.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vba.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://cfd.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lov.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://hde.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mnw.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scu.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tef.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://bqj.xinyue.icu

[E07] 按分隔符拆分
来源：http://ixm.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://njn.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pyb.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lzb.quarkkingdee.top

TS:   s.split(",")
来源：http://vpf.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://atb.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://avd.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://jod.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cdm.redwolf501.top

[E08] 数组按分隔符合并
来源：http://szp.birdmap.top

Py:   ",".join(items)
来源：http://umn.sufxvd.cn

PHP:  implode(",", $items);
来源：http://xvq.yangfankeji.com

JS:   items.join(",")
来源：http://lkm.yongpay.top

TS:   items.join(",")
来源：http://zwd.ydjk.org.cn

Java: String.join(",", items)
来源：http://cbk.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://ffz.bjfxy.top

Ruby: items.join(",")
来源：http://qpk.yonumen.top

C#:   string.Join(",", items)
来源：http://hfa.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://ssh.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sve.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jgo.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://awn.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://ymo.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://str.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fhh.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ecb.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vqc.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://mzr.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zgg.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iio.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://ibs.sweek.top

TS:   "7".padStart(3, "0")
来源：http://znn.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://hpq.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mpu.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hip.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fks.yj20258888.top

[E11] 反转字符串
来源：http://nzn.ydjk.org.cn

Py:   s[::-1]
来源：http://pkl.jianghu66.top

PHP:  strrev($s);
来源：http://wwr.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://qpl.cashguo.top

TS:   [...s].reverse().join("")
来源：http://kth.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hxy.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fzx.hnqzz.top

Ruby: s.reverse
来源：http://max.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vnp.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://rtg.gaohongyu789.top

Py:   s.count("a")
来源：http://oqq.sweek.top

PHP:  substr_count($s, "a");
来源：http://ofn.bjfxy.top

JS:   s.split("a").length - 1
来源：http://djh.yj20258.top

TS:   s.split("a").length - 1
来源：http://qeb.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xdl.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://xry.yuxming.cn

Ruby: s.count("a")
来源：http://lmf.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://iif.yonumen.top

[E13] 逐字符遍历
来源：http://tas.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://kzs.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ydc.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tqc.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qll.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yww.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ihn.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dwl.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mcj.hammf.cn

[E14] URL 编码与 Base64
来源：http://hjx.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zwv.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://scr.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mka.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://joy.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sup.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ygr.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jae.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vee.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://alm.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rod.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ies.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xhk.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lhh.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zac.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://myv.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bux.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ngn.tianlin.xyz

[E16] 数字千分位
来源：http://xhq.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://kaj.ybcxt.top

PHP:  number_format(1234567);
来源：http://aaq.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dzp.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://vsx.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pvs.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eex.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qxd.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://gpk.yj20258.top

[E17] 首字母大写
来源：http://ohx.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oub.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://evu.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uuk.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxa.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://owm.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enp.zdbjq.cn

Ruby: s.capitalize
来源：http://tzy.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vtc.quarkkingdee.top

[E18] 模板占位符替换
来源：http://zsi.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hjc.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tbn.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vqh.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mbx.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://crq.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ubu.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pqx.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qvm.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://jst.tarul.cn

Py:   s.splitlines()
来源：http://bmj.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xgs.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://ryi.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://mrs.tanke756.top

Java: s.lines().toList()
来源：http://kid.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://ybd.cheryme.top

Ruby: s.lines
来源：http://khu.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://gly.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://odl.shuidangran.top

Py:   if not s:
来源：http://yfm.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dap.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tli.yanxiufei.cn

TS:   if (s === "") {}
来源：http://zsp.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://exm.jianghu66.top

Go:   if s == "" {}
来源：http://hat.zhongyouzk.top

Ruby: if s.empty?
来源：http://lwi.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cfr.iojbl.cn

[E21] 超长截断加省略号
来源：http://lcv.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xrh.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xwy.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hzs.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsh.zhoulong.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lup.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://hix.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kzv.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zkz.daxiang520.top

[E22] 字节长度与字符长度
来源：http://bnm.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vua.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vwj.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ujl.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehe.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ryq.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sna.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://gle.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izn.cucudq.cn

================================================================================
来源：http://sow.xinyue.icu

F. 文件与目录
来源：http://ery.xuanzx.com

================================================================================
来源：http://ojc.ybcxt.top

[F01] 读取整个文件
来源：http://wll.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ryc.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://soc.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oaj.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tyh.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pdq.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://njy.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://mfk.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://jhg.xylfe.cn

[F02] 逐行读取文件
来源：http://zmx.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qjj.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vwr.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aln.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhb.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dhq.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jph.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hoj.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lut.tanke756.top

[F03] 写入文件（覆盖）
来源：http://ztc.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://flh.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hmw.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://syf.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uis.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tgi.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gpf.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://que.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://slu.jinqigfzy.top

[F04] 追加写入文件
来源：http://xsx.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uox.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tgh.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cox.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://smy.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vca.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://euy.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lfh.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fja.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://omd.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxi.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://skc.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://afc.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://zcu.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vuo.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sba.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://sgl.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://ray.tarul.cn

[F06] 删除文件
来源：http://mvn.guannengcc.top

Py:   os.remove("a.txt")
来源：http://wxa.cheryme.top

PHP:  unlink("a.txt");
来源：http://uuu.hnqzz.top


<!-- 参考信息 -->