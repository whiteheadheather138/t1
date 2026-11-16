代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iir.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://miq.tanke756.top

C#:   list.Max();  list.Min()
来源：http://usy.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://lbh.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qje.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://mge.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gki.hongshengwenyu.top

TS:   nested.flat();
来源：http://xbw.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gja.zhijiandao.cn

Go:   // 手写双层循环
来源：http://tdr.hywenlv.cn

Ruby: nested.flatten
来源：http://als.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xbt.mhx1999.top

[D19] 按字段分组
来源：http://ofe.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mmd.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dlo.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxi.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sbb.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ucm.ivvv.top

Go:   // 手写 map[string][]T
来源：http://fgv.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hzo.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jgw.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://rtp.316326.xyz

Py:   Counter(arr)
来源：http://hns.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://axu.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xyh.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tjk.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nkc.xylfe.cn

Go:   // 手写 map[T]int
来源：http://ceu.yj202588.top

Ruby: arr.tally
来源：http://ogx.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oqg.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://otq.ywan-chungtsiang.top

Py:   x in arr
来源：http://cby.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://fpl.zycfv.cn

JS:   arr.includes(x)
来源：http://rbp.ivvv.top

TS:   arr.includes(x)
来源：http://his.gaohongyu789.top

Java: list.contains(x)
来源：http://frf.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://vga.ydzc1.top

Ruby: arr.include?(x)
来源：http://smp.andypj.xyz

C#:   list.Contains(x)
来源：http://gbi.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://ogi.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iax.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rth.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bbu.vehdjk.com

TS:   [...arr];
来源：http://akx.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://fqu.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://gxd.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://gjf.epnwcf.com

C#:   new List<int>(list);
来源：http://tuh.guowangkeji.top

[D23] reduce 累积计算
来源：http://glu.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wqo.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eqd.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwj.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivg.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ylx.jqgfzy.top

Go:   // 手写循环
来源：http://gkb.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://udz.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvr.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://fyt.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uta.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qco.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rfj.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://olf.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://laa.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ags.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wbf.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oix.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://qmz.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kkg.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ray.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://smk.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bbf.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://app.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://voa.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nnn.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ljn.smart0.xyz

[D26] 数组转字符串
来源：http://peh.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://fch.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://blh.hnqzz.top

JS:   arr.join(", ")
来源：http://ema.cheryme.top

TS:   arr.join(", ")
来源：http://wgf.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://vdo.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://etr.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://nya.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://ife.andypj.xyz

================================================================================
来源：http://urq.meibo888.top

E. 字符串处理
来源：http://uxh.sxryk.cn

================================================================================
来源：http://pzs.shangyingyoupin.top

[E01] 拼接字符串
来源：http://imx.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pds.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ija.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://toh.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcd.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mwe.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hty.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nio.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fkx.smart0.xyz

[E02] 重复字符串
来源：http://oke.fktsv.cn

Py:   "ab" * 3
来源：http://ieu.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://fnv.yongpay.top

JS:   "ab".repeat(3)
来源：http://lug.fehbvm.com

TS:   "ab".repeat(3)
来源：http://mgm.zhengqikj.top

Java: "ab".repeat(3)
来源：http://vbo.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://uhm.yj20258.top

Ruby: "ab" * 3
来源：http://ula.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://azn.yonumen.top

[E03] 截取子串
来源：http://wlx.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://znt.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqq.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zlf.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://jqh.andypj.xyz

Java: s.substring(1, 4)
来源：http://scu.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://esq.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://xmv.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://tbg.hysaishi.cn

[E04] 查找子串位置
来源：http://zzf.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://vzx.ydzc1.top

PHP:  strpos($s, "x");
来源：http://pat.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xay.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://bui.zycfv.cn

Java: s.indexOf("x")
来源：http://jue.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://hwg.zhiwuduotai.top

Ruby: s.index("x")
来源：http://qwd.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://lec.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://owy.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oeq.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jfg.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gom.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://yvk.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gcw.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xxs.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rtc.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ivq.sxryk.cn

[E06] 替换子串
来源：http://doh.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bmx.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://ubb.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufr.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://dgq.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ucu.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dvn.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dgj.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://tyq.sysykeji.top

[E07] 按分隔符拆分
来源：http://bms.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdo.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hxe.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gvm.hammf.cn

TS:   s.split(",")
来源：http://hvy.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://gge.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bkn.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://typ.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://axh.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://ifg.chenjidiqi.icu

Py:   ",".join(items)
来源：http://yrg.uphjek.com

PHP:  implode(",", $items);
来源：http://zyq.zhijiandao.cn

JS:   items.join(",")
来源：http://roz.haohaochexian.top

TS:   items.join(",")
来源：http://ttc.fzhhl.top

Java: String.join(",", items)
来源：http://qqk.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://xqn.chenlongwang.top

Ruby: items.join(",")
来源：http://pdn.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://bgz.aibaodan.cn

[E09] 去除所有空白字符
来源：http://scm.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lrt.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpw.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://kfp.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://omh.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://rib.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uuu.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://rsi.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycm.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://fla.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qwl.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://apw.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://ljj.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://lua.daxiang520.top

Java: String.format("%03d", 7)
来源：http://ptx.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gvv.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lye.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jcy.jqgufenzy.top

[E11] 反转字符串
来源：http://hjf.yueranfly.top

Py:   s[::-1]
来源：http://wzl.zdqjudy.top

PHP:  strrev($s);
来源：http://cnx.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://jnu.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://tro.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nws.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tyh.jqgfzy.top

Ruby: s.reverse
来源：http://cnd.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://dnz.yfazqb.com

[E12] 统计某字符出现次数
来源：http://nvm.sufxvd.cn

Py:   s.count("a")
来源：http://dtj.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://eik.aizwys.cn

JS:   s.split("a").length - 1
来源：http://czz.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://vyf.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://stk.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://kea.iojbl.cn

Ruby: s.count("a")
来源：http://jvb.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://dhn.sweek.top

[E13] 逐字符遍历
来源：http://fmh.yj202588.top

Py:   for ch in s: print(ch)
来源：http://vfh.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ujm.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://swg.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kgi.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wxq.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rgt.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rls.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hhl.ybcxt.top

[E14] URL 编码与 Base64
来源：http://ksn.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rfw.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bvk.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jht.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eih.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://npp.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqc.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vah.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://huu.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://pqu.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pbx.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dub.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://csl.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ozl.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ynh.xylfe.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ztj.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://npr.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hsx.jqgufenzy.top

[E16] 数字千分位
来源：http://zyp.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://yan.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://trc.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aok.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iha.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://toj.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ikl.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wyh.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://rzq.vqdsnc.cn

[E17] 首字母大写
来源：http://coa.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xvc.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uvq.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eiw.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oim.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qgz.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xaw.birdmap.top

Ruby: s.capitalize
来源：http://cyu.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xmc.jinqigufen.top

[E18] 模板占位符替换
来源：http://wuf.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://twb.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aax.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fin.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lxt.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ayn.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nup.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yxr.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qnd.fktsv.cn

[E19] 多行文本按行拆分
来源：http://dcx.ctjpmb.com

Py:   s.splitlines()
来源：http://bxf.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ubj.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://nzx.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://idc.epnwcf.com

Java: s.lines().toList()
来源：http://aeo.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://bns.chenjidiqi.icu

Ruby: s.lines
来源：http://vkt.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://eej.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://wkv.vqdsnc.cn

Py:   if not s:
来源：http://ndy.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bkg.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ulo.9152youxi.cn

TS:   if (s === "") {}
来源：http://tyi.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://azj.yj20258888.top

Go:   if s == "" {}
来源：http://xei.haohaochexian.top

Ruby: if s.empty?
来源：http://rxk.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://chk.yuanzhike.top

[E21] 超长截断加省略号
来源：http://wnm.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://grc.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lfz.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rzl.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pok.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cud.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://sui.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uln.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aqh.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://mzc.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzs.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://png.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhj.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uje.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://deq.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcd.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://vci.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xjk.pycfn.com

================================================================================
来源：http://dlj.guowangkeji.top

F. 文件与目录
来源：http://sks.gaohongyu789.top

================================================================================
来源：http://jqg.fzhhl.top

[F01] 读取整个文件
来源：http://dme.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ygt.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://ctl.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zeq.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vnr.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nrd.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fyc.c1oappe.top

Ruby: File.read("a.txt")
来源：http://gmh.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://rjy.316326.xyz

[F02] 逐行读取文件
来源：http://awm.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rwz.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://azo.sjlbkw.cn


<!-- 参考信息 -->