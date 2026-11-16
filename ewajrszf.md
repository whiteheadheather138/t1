代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gwh.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://axf.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://jko.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://xjm.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ipb.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://zab.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://das.guannengcc.top

TS:   nested.flat();
来源：http://jle.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://syb.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://iuh.kuanghao11.cn

Ruby: nested.flatten
来源：http://qll.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uij.sysykeji.top

[D19] 按字段分组
来源：http://rlt.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mnx.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://snr.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dha.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dqq.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nzp.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://ujl.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpz.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gbo.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://csb.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://afb.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://dwt.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kca.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gql.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dcw.smart0.xyz

Go:   // 手写 map[T]int
来源：http://mfi.bbcook.cn

Ruby: arr.tally
来源：http://pdl.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hdt.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://dyg.jinyuanbaomall.cn

Py:   x in arr
来源：http://vni.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://xfm.havefunace.top

JS:   arr.includes(x)
来源：http://shh.0kj1m.cn

TS:   arr.includes(x)
来源：http://mqz.hcnkem.com

Java: list.contains(x)
来源：http://znk.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://tfs.bbcook.cn

Ruby: arr.include?(x)
来源：http://bfe.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://qgh.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://mxr.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uxj.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zrb.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ufw.yj202588.top

TS:   [...arr];
来源：http://lur.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://pjg.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://imn.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://vel.hywenlv.cn

C#:   new List<int>(list);
来源：http://ydk.tarul.cn

[D23] reduce 累积计算
来源：http://xtn.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ese.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zmt.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbx.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ylc.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyl.zhiwuduotai.top

Go:   // 手写循环
来源：http://umx.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gzm.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wfi.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://poi.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bhn.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://imy.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfk.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mhi.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ulj.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qpn.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zhu.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://apu.yj20258.top

[D25] Set 集合去重与交并差
来源：http://rwq.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzc.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://afg.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vvy.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jax.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vpy.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vxl.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wbg.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://csn.sweek.top

[D26] 数组转字符串
来源：http://zyl.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://fce.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://zdl.tarul.cn

JS:   arr.join(", ")
来源：http://kau.xylfe.cn

TS:   arr.join(", ")
来源：http://kab.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://inn.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://wgw.smart0.xyz

Ruby: arr.join(", ")
来源：http://jpb.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://bbv.aibaodan.cn

================================================================================
来源：http://tlk.jqgfzy.top

E. 字符串处理
来源：http://mll.jianghu66.top

================================================================================
来源：http://hkg.tianlin.xyz

[E01] 拼接字符串
来源：http://xdj.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tro.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fdh.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kqw.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hap.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mmz.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nwm.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nxp.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uwc.ppjwa.cn

[E02] 重复字符串
来源：http://wpy.ydzc1.top

Py:   "ab" * 3
来源：http://pes.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://mla.xuanzx.com

JS:   "ab".repeat(3)
来源：http://dzv.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://ewu.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://pyp.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://pzr.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://dcl.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yqn.xuetiantiany.cn

[E03] 截取子串
来源：http://pla.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lqk.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oth.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aoz.52xcode.cn

TS:   s.slice(1, 4)
来源：http://ehl.yvedp.cn

Java: s.substring(1, 4)
来源：http://hcg.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhf.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://wdn.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://chl.zhoulong.xyz

[E04] 查找子串位置
来源：http://dnc.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://prn.yj20258888.top

PHP:  strpos($s, "x");
来源：http://kfw.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://htd.shzxlz.cn

TS:   s.indexOf("x")
来源：http://gim.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://tch.birdmap.top

Go:   strings.Index(s, "x")
来源：http://kgn.yj20258888.top

Ruby: s.index("x")
来源：http://jcj.yueranfly.top

C#:   s.IndexOf("x")
来源：http://kkp.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dsu.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tbt.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ixn.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzg.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lke.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbq.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://njv.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sos.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iem.ivvv.top

[E06] 替换子串
来源：http://vbn.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rdt.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://bqz.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xqv.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://gjl.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojv.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cty.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://twe.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://cfc.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://vwl.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mce.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lrm.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ylo.yongpay.top

TS:   s.split(",")
来源：http://zue.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://tsj.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qqd.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://ltm.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rzi.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://vrt.yueranfly.top

Py:   ",".join(items)
来源：http://byk.pycfn.com

PHP:  implode(",", $items);
来源：http://ocy.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://vxc.hywenlv.cn

TS:   items.join(",")
来源：http://wjv.redwolf501.top

Java: String.join(",", items)
来源：http://gkz.hammf.cn

Go:   strings.Join(items, ",")
来源：http://xkp.hesvh.cn

Ruby: items.join(",")
来源：http://pwg.zhengqikj.top

C#:   string.Join(",", items)
来源：http://vfj.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://vkw.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xsw.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fkk.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://hsm.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://zuf.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://tkj.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://izr.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://gch.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://drz.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://kzl.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sct.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ani.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://jgz.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://kmr.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://wyq.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eis.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sgt.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fge.iojbl.cn

[E11] 反转字符串
来源：http://ylr.fktsv.cn

Py:   s[::-1]
来源：http://meb.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://zko.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://ylj.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://noq.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mhl.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xrj.sweek.top

Ruby: s.reverse
来源：http://qem.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://kqc.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://xdc.nanxuanxn.top

Py:   s.count("a")
来源：http://woz.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://smc.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://anu.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://xov.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://crv.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://xbl.hongshengwenyu.top

Ruby: s.count("a")
来源：http://lqf.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://lof.hysaishi.cn

[E13] 逐字符遍历
来源：http://lhe.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://wyu.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xvl.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qyk.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://aav.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://piz.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://syu.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ejp.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://adg.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://cwv.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cbq.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://apg.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cyh.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pet.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvb.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pbu.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xts.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://egg.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://vpm.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aub.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lab.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ymm.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nee.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rzl.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cdg.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dkx.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://klb.jinqigfzy.top

[E16] 数字千分位
来源：http://sdg.meibo888.top

Py:   f"{1234567:,}"
来源：http://pnb.chenzaomai.com

PHP:  number_format(1234567);
来源：http://kbd.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://vge.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yaq.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dhy.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://izi.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ftz.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://vgu.shuidangran.top

[E17] 首字母大写
来源：http://xvl.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zap.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://utf.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mtf.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kcr.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hjm.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://okd.dashuyun.cn

Ruby: s.capitalize
来源：http://tfx.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eqx.xylfe.cn

[E18] 模板占位符替换
来源：http://ctn.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tus.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vor.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://byg.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mpl.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgl.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rae.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xuk.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kbe.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://yqf.sufxvd.cn

Py:   s.splitlines()
来源：http://zcm.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sgk.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://kcx.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://iob.zhiwuduotai.top

Java: s.lines().toList()
来源：http://kxl.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://rqp.aizwys.cn

Ruby: s.lines
来源：http://plv.nanxinkj.top

C#:   s.Split('\n')
来源：http://cth.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://tph.quarkkingdee.top

Py:   if not s:
来源：http://ihg.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://abb.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jqy.c1oappe.top

TS:   if (s === "") {}
来源：http://mgh.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://gnv.zhongyouzk.top

Go:   if s == "" {}
来源：http://dqo.jinqigufen.top

Ruby: if s.empty?
来源：http://nkd.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kpm.nanxinkj.top

[E21] 超长截断加省略号
来源：http://iwa.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ytp.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nmu.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yar.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xsc.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gds.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://zoa.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ihm.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxs.ybcxt.top

[E22] 字节长度与字符长度
来源：http://qao.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hjh.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gmv.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ash.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyp.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gjn.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://upa.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://zae.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://boh.jinqigfzy.top

================================================================================
来源：http://juu.meibo888.top

F. 文件与目录
来源：http://bms.dashuyun.cn

================================================================================
来源：http://dcg.guannengcc.top

[F01] 读取整个文件
来源：http://zim.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://myq.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://wnk.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gbv.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ncn.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hih.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nvo.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://qza.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://pgw.hnqzz.top

[F02] 逐行读取文件
来源：http://dka.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xby.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ioq.tianlin.xyz


<!-- 参考信息 -->