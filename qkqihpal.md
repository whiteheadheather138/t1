代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tzx.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://htk.feifeiyinyue.top

Py:   Counter(arr)
来源：http://jfg.cheryme.top

PHP:  array_count_values($arr);
来源：http://uqy.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zgz.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ves.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tli.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://qkt.hesvh.cn

Ruby: arr.tally
来源：http://elr.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://got.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://pcr.aizwys.cn

Py:   x in arr
来源：http://usg.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://zyh.cucudq.cn

JS:   arr.includes(x)
来源：http://dpo.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://fts.jinqigfzy.top

Java: list.contains(x)
来源：http://cya.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://iff.hywenlv.cn

Ruby: arr.include?(x)
来源：http://cwx.ppjwa.cn

C#:   list.Contains(x)
来源：http://igq.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://njv.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aqe.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ntp.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://plt.jinqigfzy.top

TS:   [...arr];
来源：http://zrv.fengsongda.top

Java: new ArrayList<>(list);
来源：http://oir.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://mvu.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://ysa.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://dpd.xziqi.cn

[D23] reduce 累积计算
来源：http://hyf.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://clv.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lbi.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rwa.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqc.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://nlv.yueranfly.top

Go:   // 手写循环
来源：http://ywk.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://riq.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eqe.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://mmn.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pld.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vnz.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gma.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uez.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cwd.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gbn.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqe.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kqi.cheryme.top

[D25] Set 集合去重与交并差
来源：http://zid.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lzj.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pqx.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jbv.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tsx.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ekf.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pme.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oaq.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rgi.yanxiufei.cn

[D26] 数组转字符串
来源：http://lew.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://jiv.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://ivj.tian-w.cn

JS:   arr.join(", ")
来源：http://tsd.yangfankeji.com

TS:   arr.join(", ")
来源：http://tbb.gaohongyu789.top

Java: String.join(", ", list)
来源：http://kvx.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://duk.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://cpj.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://vtr.haohaochexian.top

================================================================================
来源：http://cjn.c1oappe.top

E. 字符串处理
来源：http://mbf.tian-w.cn

================================================================================
来源：http://vhc.snrcjt.cn

[E01] 拼接字符串
来源：http://bxv.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plc.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wbp.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrb.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uix.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://owu.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yfj.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vti.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lvj.yfazqb.com

[E02] 重复字符串
来源：http://ymg.ehwqpu.com

Py:   "ab" * 3
来源：http://rrw.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://vau.yonumen.top

JS:   "ab".repeat(3)
来源：http://adu.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://unk.iojbl.cn

Java: "ab".repeat(3)
来源：http://mvl.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://ura.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://ysi.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nqq.yanxiufei.cn

[E03] 截取子串
来源：http://wnp.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fxf.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hfd.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://itt.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://mad.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://cux.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rie.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://dtv.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://qzv.yfazqb.com

[E04] 查找子串位置
来源：http://kkg.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://rzx.nwbrower.top

PHP:  strpos($s, "x");
来源：http://dja.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vet.yuanzhike.top

TS:   s.indexOf("x")
来源：http://xwa.yuxming.cn

Java: s.indexOf("x")
来源：http://vbk.hammf.cn

Go:   strings.Index(s, "x")
来源：http://xif.nwbrower.top

Ruby: s.index("x")
来源：http://kud.iojbl.cn

C#:   s.IndexOf("x")
来源：http://tsy.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mlu.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hye.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://osv.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cgs.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbx.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ksl.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cja.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ktq.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dgh.fktsv.cn

[E06] 替换子串
来源：http://gyf.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sli.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://uly.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://acu.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://sli.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blw.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ase.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://beo.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://knp.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://zek.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tto.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zjm.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://nod.feifeiyinyue.top

TS:   s.split(",")
来源：http://fcb.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://eqv.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fnn.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://ytt.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ixe.uphjek.com

[E08] 数组按分隔符合并
来源：http://eum.jianghu66.top

Py:   ",".join(items)
来源：http://hdi.jianghu66.top

PHP:  implode(",", $items);
来源：http://tkj.gotoacloud.top

JS:   items.join(",")
来源：http://hgu.ehwqpu.com

TS:   items.join(",")
来源：http://mir.jinqigufen.top

Java: String.join(",", items)
来源：http://azm.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://vtx.yj20258.top

Ruby: items.join(",")
来源：http://jcu.smart0.xyz

C#:   string.Join(",", items)
来源：http://mzs.zhixingplan.top

[E09] 去除所有空白字符
来源：http://mvi.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hut.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zat.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://ghm.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://txy.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://pbn.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ahp.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://kow.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ecg.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://kat.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kwo.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://trh.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://zsp.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://yeu.meibo888.top

Java: String.format("%03d", 7)
来源：http://dnu.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lsu.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gmf.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kbo.haohaochexian.top

[E11] 反转字符串
来源：http://tgh.ybcxt.top

Py:   s[::-1]
来源：http://vdk.cashguo.top

PHP:  strrev($s);
来源：http://fkt.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://tcb.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://asl.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pqg.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ivv.jlsjyb.cn

Ruby: s.reverse
来源：http://gia.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://mww.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://vwh.gogol.net.cn

Py:   s.count("a")
来源：http://ppz.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://cob.meibo888.top

JS:   s.split("a").length - 1
来源：http://vwm.yongpay.top

TS:   s.split("a").length - 1
来源：http://pvh.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vxp.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://bud.tian-w.cn

Ruby: s.count("a")
来源：http://osr.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://txq.redwolf501.top

[E13] 逐字符遍历
来源：http://cgu.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://ves.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zri.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xrm.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://krh.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uby.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zve.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xpe.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://des.guannengcc.top

[E14] URL 编码与 Base64
来源：http://mdo.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://efy.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tob.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ruh.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rbc.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zwz.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xag.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qdz.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hhl.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://ezy.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://bop.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tzh.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iqz.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fbm.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xgi.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yfg.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://crs.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gfz.birdmap.top

[E16] 数字千分位
来源：http://zaa.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://lkz.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://bhv.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cam.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jyn.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xwv.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ymu.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eaw.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://odl.gotoacloud.top

[E17] 首字母大写
来源：http://jqq.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://btq.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nyp.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nht.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djw.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jut.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zzo.yfazqb.com

Ruby: s.capitalize
来源：http://rlf.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://joc.yj20258888.top

[E18] 模板占位符替换
来源：http://amx.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tcd.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qct.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pai.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ofl.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nhg.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uhq.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jde.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hcx.ydzc1.top

[E19] 多行文本按行拆分
来源：http://owp.yuxming.cn

Py:   s.splitlines()
来源：http://woj.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lvn.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://xtm.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://srp.jyoumei.cn

Java: s.lines().toList()
来源：http://ewe.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://yrp.redwolf501.top

Ruby: s.lines
来源：http://bpg.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://ecn.yvedp.cn

[E20] 判断字符串是否为空
来源：http://wce.ppjwa.cn

Py:   if not s:
来源：http://ohq.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbq.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oqd.epnwcf.com

TS:   if (s === "") {}
来源：http://utz.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://gez.havefunace.top

Go:   if s == "" {}
来源：http://yfm.yj20258888.top

Ruby: if s.empty?
来源：http://eec.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xxl.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://nzi.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hyn.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tou.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsn.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hzy.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ihi.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://gfv.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bwq.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://etk.ybcxt.top

[E22] 字节长度与字符长度
来源：http://jcw.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://orw.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://knm.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrh.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vad.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyf.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zkp.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://eae.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ans.jinghuilouyu.cn

================================================================================
来源：http://btl.zhengqikj.top

F. 文件与目录
来源：http://fuv.sweek.top

================================================================================
来源：http://jqf.jyoumei.cn

[F01] 读取整个文件
来源：http://gdv.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kan.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://fvj.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sec.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rwe.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://inl.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qee.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://ody.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://lka.zhijiandao.cn

[F02] 逐行读取文件
来源：http://kfj.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xec.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://skl.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqo.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjg.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mec.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ksj.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lgd.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yrj.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://jvt.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pfp.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kcj.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kac.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yex.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gnb.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tha.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://gre.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tmo.meibo888.top

[F04] 追加写入文件
来源：http://csc.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ywr.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yer.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fda.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfs.havefunace.top


<!-- 参考信息 -->